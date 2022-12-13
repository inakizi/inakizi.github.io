---
layout: post
title: Take your High Reliability Control System to the Stars
subtitle: By Iñaki Zuloaga (IZI) CTO IOT-eq
date: June 23, 2020
---

When I started at IOT-eq a little over 2 years ago, the first thing I did was to distribute copies of “The Power of 10: Rules for Developing Safety-Critical Code” among our developers. These rules showed in an article written in 2006 by Gerard J. Holzmann from NASA/JPL. Then while reading a Q&A by SpaceX engineers about the software architecture used for the successful Demo 2 launch, I find out that they always use these same rules for developing their software.

And that was just the start, similarities from IOT-eq software and system design to those used by SpaceX are startling. This article highlights some similarities between our systems and SpaceX’s as a guide to keep doing all the things we are doing right.

**Detached HMI process using Chromium, HTML, and JavaScript.** Web technologies have achieved a top level of maturity after many years of worldwide use. As SpaceX does, IOT-eq uses in all our new HMIs a Linux based industrial panel PC running Chromium. HTML and JavaScript developed pages show a modern view of your control system. This architecture detaches user interaction from the control system, providing a safe, modern, and highly efficient way to display information without risking your process.

**Multiprocessing.** In the SpaceX Q&A, they mention that in a Starlink network, composed of 60 satellites, over 4,000 Linux computers are in use. In their current 362 satellites network there are 30,000 Linux computers and 6,000 Microcontrollers in use. This way of dividing tasks among multiple similar processors is something IOT-eq does and recommend in our customer architectures. Just to give a few examples, each one of our Duro1 control platform contains 5 Microcontrollers taking care of the IO and 1 two core Linux processor. Some smaller systems we have created for our customers have 5 Linux computers and at least 12 Microprocessors running in a seamless high-reliability dance.

**Sharp division between software and configuration.** Some developers believe in monolithic software specifically created with one application in mind. But monolithic software is hard to maintain and not portable among customers. The same way that SpaceX does, IOT-eq divides Software in Base Software and Configuration. Every SpaceX mission has a unique configuration holding guidance and navigation parameters, in the same way every project made by IOT-eq has a configuration as unique as the customer system. This customer configuration is our customer IP and runs only on customer systems. However, our base Software is a multipurpose software that keeps getting better and more reliable because we build on it. Unlike SpaceX, where every mission has a better chance of success but cannot change past launches, IOT-eq distributes Software upgrades to our customers to make their control systems better every day.

But enough of technobabble. What does these similarities mean for our customers? Using technology just for the sake of it is not good enough, it has to offer tangible benefits. By applying proven technologies, used to send people to space, you guarantee that your control system is future proof, stable, and maintainable. These are the cornerstones of a successful control system that will save you and your employees many headaches.

By learning every day, applying continuous improvement in everything we do, and following the footsteps of giants, IOT-eq brings the best technology available to the oil field and its customers.

## References: 
G.J. Holzmann (2006-06-19). "The Power of 10: Rules for Developing Safety-Critical Code". IEEE Computer. 39 (6): 95–99. doi:10.1109/MC.2006.212. [Non-paywalled version](http://web.eecs.umich.edu/~imarkov/10rules.pdf)

[We are the SpaceX software team, ask us anything!](https://www.reddit.com/r/spacex/comments/gxb7j1/we_are_the_spacex_software_team_ask_us_anything/)

