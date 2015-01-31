---
layout: page
title: About Me
modified: 2015-01-30T20:53:07.573882-04:00
comments: true
image:
  feature: sample-image-2.jpg
  credit: WeGraphics
  creditlink: http://wegraphics.net/downloads/free-ultimate-blurred-background-pack/
---

I'm a data scientist at [Swipely](http://swipely.com/), where I love helping our merchants learn more about how their businesses tick.
I can't help but tinker on a steady stream of software projects on the side as well, and some of my favorites are linked below.

With what remains of my free time, I'm an avid musician.
I play guitar and sing in the [Eric Barao band](http://ericbarao.com/), and I've been teaching myself the pedal steel for the last year or so.

Views expressed here are my own, and I've got the receipts to prove it.

## Assorted Projects:

{% for project in site.data.projects %}
* [{{ project.title }}]({{ project.external_url }}) &mdash; {{ project.description }}{% endfor %}
