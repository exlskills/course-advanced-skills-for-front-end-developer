## Why Browser Needs CPU

The browser is a program that (1) converts HTML/CSS sent from the website into
screen pixels (whatever the video card/screen driver need to do their work) and
(2) runs other programs that the website submits to it in the form of JavaScript
(JS). So, if the website pushes lots of JS code to the browser, the latter is
going to get busy cranking through the device’s resources and energy. Here comes
a great analogy coined in the software industry between JS and environmental
pollutants accelerating global warming.

As already explained, the JS code will take longer to complete on a phone vs. a
computer. What does this mean for an FE developer? Test and benchmark your
prototype on a slow phone (emulator) first. If the design holds, proceed with
the development, otherwise – redesign, basically, select a strategy minimizing
the use of JS.