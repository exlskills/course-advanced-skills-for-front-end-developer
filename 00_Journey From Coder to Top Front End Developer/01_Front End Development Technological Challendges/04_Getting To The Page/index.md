## Initial Page Load vs. Navigation

In addition to CPU and network, the browser has access to the local memory and
some disk space on the device. When the browser first gets to a site’s page,
e.g., when the user clicks on the link in the search engine, this is considered
an *initial page load* - as the browser doesn’t have any data related to the
site in its memory or on disk. Once the initial page is loaded, further work
with the site is done via the *navigation*. If the site’s pages are fairly
consistent in design and functionality, during the navigation, the browser would
only need to load the content and JS that wasn’t loaded earlier with other
pages. As well, it may only need to *paint* just a section of the page vs.
repainting the entire screen. So, there is a potential difference in the state
of the browser and behavior of the page depending on whether the page was
accessed from an external link or navigated to via another page of the site.

It is important to know that Search Engine bots always load pages as in the
external link access scenario, one at a time, vs. navigating between them. Once
the page is loaded, the bot looks over it for links to other pages, loads those,
etc. A pretty boring process.

For the browser, the obvious concern with the initial page load is the amount of
time it takes getting all the page’s components via the network vs. from the
on-device storage and compiling the JS before it can be executed. In reality,
the browser may have *cookies* and/or files (graphics, JS libraries) stored on
the disk from earlier visits to this or similar sites.
