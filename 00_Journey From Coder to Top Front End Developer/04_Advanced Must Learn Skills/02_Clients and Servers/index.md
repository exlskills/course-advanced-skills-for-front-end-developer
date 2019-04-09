## Networking and Client-Server/Browser-API Communications

A good trick for promoting some technology is to give it a new name. Something
*new* got to be *different and better*. There is a popular movement that labels
everything with the word “server” in it as being bad and old-style. Sure, a
bulky component that requires setup, configuration, maintenance is no longer the
only way of providing computing services. However, the concept of the browser
being a *client* and needing a *server* to operate didn’t go away – it hasn’t
changed much either (well, except, maybe, for a small subset of apps that don’t
do anything). Communications with the server can be called *API* - doesn’t
change the nature of those being done over the *network*. The impact of the
network, especially its *last mile* to the user’s device must be taken into
consideration when implementing the FE.

The network is a classic component that requires a stellar application to be
coded with breakages in mind: can the application be useful if the network is
intermittent or slow? Should critical info be re-submitted if the communication
timed out? It is easy to write an app for *ideal* conditions – can be much more
complicated for *real use* scenarios.

The biggest mistake for an FE developer can be looking at the API (server) as a
black box. The *cost* of each particular API call must be understood to code the
FE more efficiently. That includes the time the API call is executed on the
server and the amount of data being returned. More on this below.