## Caching and Memory Management

Caching is the key thing in today’s software. Each component either does caching
or will do soon.

The database uses advanced caching. The server/CDN (good ones) caches the last
retrieved and/or most frequently used responses and content. The browser caches
anything it can. The JS framework caches received data. Proper use of cache can
speed up the application tremendously. Of course, not all Use Cases can take
advantage of caching. Then there is also pre-caching – pre-loading.

JS frameworks come equipped with runtime data storage. It is up to the FE
developer to decide what to put into it, for the most part. More stuff is loaded
and cached – more memory is used.

The careful planning and testing of the calls, paging size of data being pulled
is a necessity to ensure the positive UX (User eXperience).
