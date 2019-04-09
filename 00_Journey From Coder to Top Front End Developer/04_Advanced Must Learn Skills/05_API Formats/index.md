## Common API Formats

In a typical modern web application, JS code running in the browser sends and
receives data from servers. The data exchange can be done via custom formats and
methods or by adhering to industry-standard API ones. Custom-formatted calls via
*jQuery* is a popular option when the application is developed by a small team
and/or the server side is implemented for internal use only. Common API formats
used in standard software are REST and GraphQL. The SOAP standard has been
around as well, but as it is overly complex, slow and bulky – it would not be
used for browser-server communications within a single web application. There is
not much special about REST, which stands for Representational State Transfer
and is a part of *RESTful Web Services*: the communications are done by issuing
HTTP calls and there are a few common ways the calls should be formatted to; the
actual data is passed as JSON, as well as HTTP call parameters.

There is a lot of hype around GraphQL. It is usually implemented within a
complete client-server framework which abstracts the HTTP calls from the
developers. There are many interesting and useful features in GraphQL, although,
the development requires understanding how the framework operates and coding to
its syntax and rules. GraphQL is very popular and the use of it is growing, but
it is surely not the *necessity* when writing a data exchange API. Once it peaks
at some point, it may likely fade away in the direction SOAP went: developers
hate doing extra work adhering to something they may get by without.
