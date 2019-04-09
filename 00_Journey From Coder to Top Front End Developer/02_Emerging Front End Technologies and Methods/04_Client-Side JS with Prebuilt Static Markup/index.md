## Client-Side JS with Prebuilt Static Markup

Historically, there was a short period of time when early web servers could only
really pass static content to the browser. *CGI Scripting* was the first
official method of adding dynamic capabilities, once it’s got more or less
manageable – barely a notch over being total torture to work with.

20 years later, developers realized that for sites which provide static or
periodically updated content, like Content Management Systems (CMS), pages can
be pre-generated at build time and then served *statically* at runtime, from a
CDN. In this approach, JS included in the pages provides capabilities to manage
user interaction and API-style data exchanges from the browser directly –
similarly to the SPA concept. Unlike in SPA, the JS work, though, is focused on
managing the flow vs. updating the DOM and painting pages. Thus, the load speed
and SEO friendliness are both high. The downside: changes in content that need
to be reflected in pre-generated pages require re-build/regeneration. So, this
technology is effective for some types of sites but would not work for others.

Now that we reviewed the options, let’s see if we can answer the core question
next.
