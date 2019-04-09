## Single Page Application (SPA)

The navigation functionality enables the design known as SPA: the entire
application is written as one HTML file with (lots) of JS attached to it, which
includes the *router* code. When such a page is *loaded* via any link (or URL),
it loads its core into the browser and the browser starts executing the JS code
that processes the logic of painting the page as per the navigation part of the
URL - *client-side routing*. The loaded JS code also paints pages via directly
building and updating the DOM. Further clicks on the page go through the
client-side routing as well, so no more *pages* are ever loaded again from the
server – here’s the SPA name.

The obvious downsides of SPA are:

-   bots skip the page

-   it takes a long time to load the initial page, compile and start its JS
    engine and client-side navigation before painting the first page for the
    user

-   depending on the complexity, the SPA may require significant CPU and memory
    resources of the browser

What’s good about SPA:

-   no need to maintain the server infrastructure to produce pages for clients –
    the server, if any, would only be utilized to manage dynamic data exchanges.
    The user, of course, doesn’t really care about this benefit, unless the
    savings are passed on to the user base in the form of better service, etc.

-   no need to ping the server each time the user navigates within the site,
    other than facilitating dynamic data exchanges
