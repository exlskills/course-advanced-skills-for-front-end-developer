## The Product Must be Good On Any User Hardware

A nice thing about developing application software since the time the Assembly
language was superseded by human-readable ones some 50 years ago - the code
would generally run on any hardware, within some scope, of course. Yes, there
has been a reasonable separation of software development by the size of the
hardware applications would run on, e.g., large machines vs. PC-like ones, as
well as the task of porting applications across different Operating Systems. But
none of that comes even close to the demand that today’s FE Development must
fulfill: implement products that run equally well on any device that users may
have - by power, capability, size, platform, etc. And do it from a single
version of a product, minimizing the need to write and maintain multiple flavors
by the target.

Technologically, the possibility of the one-version-fits-all approach comes from
the designation of the *browser* as the equalizer across all the variables.
Today’s browser is already the de-facto standard user interface on computers,
and there is a clear tendency of it gaining the same status on *handheld*
devices, including smartphones: the shift away from so-called *native*
applications in favor of unifying UI/UX on the browser is happening fast. On
phones now, web applications can not only run well in an open browser but be
*installed* on the device and run in the background like native ones as well –
the concept of Progressive Web Apps (PWA).

What does this mean for the FE developer? Ability to write effective
single-version browser-based applications that work well on any hardware
platform becomes key. And it is not just about the *look and feel* of the
application across different devices - the problem that the UI/UX designer must
address. It is about managing and optimizing the software so it can operate on
devices with inherently limited networking and computing power as effectively as
it runs on a massive development workstation. Let’s cover this next.
