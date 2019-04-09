### Multithreading and Concurrency

Every FE developer knows, of course, that JS is pseudo-multithreaded by design:
anything can be started using callbacks or Promises, and the engine will work on
all of it in parallel, little by little. What works well on a computer with
unlimited resources and designated hardware per function, may behave differently
on a phone where even seemingly unrelated functionality like network
communications, screen interactions, memory I/O, browser internal operations and
JS runtime may get throttled together in the metered processing unit, along with
the ongoing native background processes.

Another exposure of FE development to multithreading is the concept of PWA
mentioned earlier in which the JS *service worker* coded and delivered with the
application acts as a constantly running background process, even when the
browser is not active.
