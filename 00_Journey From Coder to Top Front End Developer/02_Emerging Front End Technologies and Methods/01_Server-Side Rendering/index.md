## SPA With Server-Side Rendering (SSR)

With Server-Side Rendering, the initial page load request is always processed by
the server. Ability to execute JS on either client or server is the essence of
this functionality – the server renders the SPA the same way the browser would
and sends a ready-to-paint page to the client. The browser can display the page
right away, and the bots see its content. The page comes with all the complex JS
to handles the SPA process as well as the data that the browser would obtain or
generate if it was rendering the page from scratch. So, upon receiving the page,
before the user navigation can start, the browser has to digest the JS and build
up the internal memory structure per the data received - *hydrate* the page. Any
further clicks from that point on are handled by the normal SPA logic on the
browser.

Of course, this approach requires maintaining a full server, although, it would
only be responsible for handling initial page load requests vs. the entire
navigation. The real problem is the complexity that the underlying framework has
to deal with rendering the page on the server as if it was being rendered on the
browser and then managing the hydration.
