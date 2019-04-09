## Equipped With The Knowledge – How to Pick The Right Technology For Given Use Case

With the good understanding of the Use Case and capabilities and constraints of
technology – the FE developer can choose the *right* architecture and platform
for the application. Except for some outliers, most web applications would fit
some general set of common Use Cases: they serve information, most of which is
static, record data submitted by users, display information in user-controlled
fashion.

The key decision-making points would be as follows:

-   Exposure to Search Engines

If the target business is very dependent on pages’ visibility in Search Engine
results – make every effort to architecture the site in a way that makes SEO
easy: minimize JS, serve HTML fast from the server/CDN. This pretty much means –
no SPA or SPA with SSR. Keep in mind that SSR is not always trivial or even
possible.

-   The amount of logic and data to process when painting the next page in the
    navigation mode

The initial page load performance is key for SEO as well as first-time *user
conversion*. Continuous UX is backed by how well the page-to-page navigation
works. If there is a lot of logic to process and/or data to pull from API to
paint the next page – server-side rendering may make more sense than SPA. Keep
in mind that browser DOM update minimization can be achieved when performing
server-side rendering, not just when using SPA with an advanced JS framework
like React. Processing complex logic client-side will always be slow on
hand-held devices. Pulling lots of data into the SPA defeats the advantage of
the client working with minimal over-the-network interaction with server/API.

Running and scaling a basic server can be very easy and cost-effective these
days utilizing containerization, so a hard argument against using server-side
rendering makes no sense if the UX suffers – the user will flee to competition.

-   The usage pattern of the application: peaks and drops

Logically, when most of the work is done client-side, the application is almost
immune to the volume of workloads growing during the usage peaks. Scaling
server-side is easy (as mentioned) but costs more. It lags catching up with the
demand’s growth and keeps the over-capacity longer after the usage drops. If the
navigation logic is simple and the usage pattern particularly uneven over time –
SPA makes a lot of sense.

The best approach to selecting the architecture would be prototyping a testing a
few alternatives. Go with the engineering approach, avoid blindly following
marketing hypes and “new technology” promotions.

Learn by doing, understanding and thinking, not just by listening to what and
how others do.
