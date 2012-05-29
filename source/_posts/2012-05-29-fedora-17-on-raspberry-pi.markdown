---
layout: post
title: "Fedora 17 on Raspberry Pi"
date: 2012-05-29 09:05
comments: true
categories: [fedora,arm,raspberry pi]
---
So about two weeks ago I received my
[Raspberry Pi](http://www.raspberrypi.org/). Unfortunately I've not had too
much time to actually play around with it. The day I got it I was leaving for
the [Dayton Hamvention](http://hamvention.com), so I had to get ready to go.

I had a few short hours that day, and did try out a few of the different
suggested distro images for the Pi. I first tried Fedora (the F14 remix),
then tried Debian, and I even tried Arch. They all worked (though I did have
problems with a large amount of packet loss among all of them, from the
ethernet port, but it seems to have worked itself out -- might have been a
loose connection from the cable to the router).

After trying the various distros, I left for the Hamvention (taking it with me
to show off to my friends from the
[University of Akron Ham Radio Club](http://www.w8upd.org)). But when I got
back home, it just pretty much stayed in its box. This is mostly because
I don't have an HDMI cable (I'll be ordering one next week), and so I have to
time playing with the Pi against my mom wanting to watch TV, and use the RCA
connector.

Well tonight I had an interesting idea. I was hanging out with
[KG4SGP](http://kg4sgp.com) who is in from Virginia, and we were talking about
several projects, and where the Pi might fit into them.

When I got home from hanging out, I decided that it'd be better to let my Pi
run just as a server that I can ssh into and play with, than just having it
sit in the box and doing nothing. I really do like the Pi, it's so awesome
that this little thing that can run off a USB port can run a full Linux
distro. I wanted to use it!

While I was at it, I decided I'd try to get Fedora 17 on it. I grabbed the
[latest F17 arm nightly](http://scotland.proximity.on.ca/arm-nightlies/)
(no X), flashed it to the SD card, got it booted in the Pi, set up static
networking, and got the Pi ssh-able. So now I have a Fedora 17 ARM playground.

{% img http://images.srv1.elrod.me/fedora-17-arm.png "htop" %}

{% img http://images.srv1.elrod.me/fedora-17-arm-playing-around.png "Playing around and showing off the Pi" %}

So -- Yeah. This thing is cool. Time to play with the
[GPIO pins](http://elinux.org/RPi_Low-level_peripherals#GPIO_Driving_Example_.28Python.29)
and make something cool!
