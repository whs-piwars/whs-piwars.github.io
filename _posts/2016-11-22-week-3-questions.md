---
layout: post
title: Do Androids Dream of Electric Sheep?
tags: []
bigimg: ../img/week-3-kit-completed.jpg
---

Okay, after today's meeting we've just about managed to finish assembling our mBots, so what's next?

**Let's flesh out our mBot challenges, and start thinking about what we might need to consider.**

### Line following:
One of the challenges is to
[complete five laps of a line-following course](http://piwars.org/2017-competition/challenges/line-following/),
with the fastest lap gaining the most points. We're going to figure out an algorithm to do that, using our mBots,
then rewrite it using Python when our prototype robot is ready.

* Does the width of the line make any difference?
* What difference does the number of line sensors make?
* Where should we place the line sensors, and why?
* What would happen if the line direction changed by:
  * Less than 90 degrees.
  * More than 90 degrees, but less than 135 degrees.
  * Almost 180 degrees.
* Could we cope if the lines crossed each other?
* How could we speed up subsequent runs?

### Straight-line Speed Test (Wall following):
Another challenge is the
[straight-line speed test](http://piwars.org/2017-competition/challenges/straight-line-speed-test). The course is
7.28m (24-feet) long, so either our robot has to be really accurate at going in a straight line, or we need to
use a closed-loop and correct our direction as we travel down the course.

Let's assume that our robot isn't that accurate, and use the ultrasonic sensors that come with the mBot to make sure
that we don't crash into the wall, and that we're moving in a straight line.

For the purposes of our testing, we should start out at 45 degrees to the wall, so we know we're definitely
going to crash into it, if we don't correct our course.

### But wait, what other ways are there to solve these problems?

Okay, so we've considered how me might use the sensors that come with our mBot to tackle these challenges, but
are there any other alternatives? Could we use a camera to look at the course of the line ahead of us? Could we detect
the colour underneath us in the straight-line challenge to determine whether we're going in a straight line and correct
ourselves? What about a beacon at the end of the track that we could head towards? What other alternatives are there?

---

_"Do Androids Dream of Electric Sheep?" is a novel by Philip K. Dick, which was famously used as the basis for the_
_science fiction film, "Blade Runner"._