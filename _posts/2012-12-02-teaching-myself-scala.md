---
layout: post
title: Teaching myself Scala
---

I was recently inspired to learn Scala by Matt Aimonetti's (LivingSocial) talk at RubyConf 2012: Ruby vs. the world.

<iframe width="560" height="315" src="http://www.youtube.com/embed/V_k3q37Tieg" frameborder="0" allowfullscreen></iframe>

Scala sounded like a great combination of the things I love about Ruby with the things I love about typed languages.  I could also see some upcoming challenges at [Swipely](http://swipely.com) that the language might be well-suited for.  This past Friday, we had a hack night at Swipely, which seemed like a great opportunity to get started on learning Scala.

## Lift

My first instinct was to learn Scala the way I learned Ruby:

1. Learn its most popular web framework
1. ???
1. Eventually understand language decently well

This path lead me to the [Lift web framework](http://www.liftweb.net/), currently used by Foursquare, among others.  I spent about an hour trying to find a good entry vector here, but for whatever reason, nothing was clicking.  I could tell that Lift has some cool integrations with modern browser technologies, but it was not obvious to me where to start and I grew impatient.  Someday I'll revisit Lift, but for the sake of getting something done during the hackfest, I was compelled to move on.

## Koans

I was now looking for some structure, and as you might expect from a Rubyist in this situation, I turned to TDD.  I [searched](http://duckduckgo.com) for "Scala TDD" (or something similar) and found something really cool: [Scala Koans](http://www.scalakoans.org/).

I had seen [Ruby Koans](http://www.rubykoans.com/) before, but never spent any time with them.  Apparently, this was a mistake, as this technique turned out to be a really cool way to quickly get my feet wet with Scala.

The koans are a set of automated tests which:

1. start off failing
1. run in a specific order
1. only report the first failure on each run

Your goal is to make each test pass, then move on to the next one.

The tests are organized in an order such that you start off learning the most basic parts of the language, and move on to more advanced concepts.  When necessary, the tests have comments to help guide you in the right direction.  I was able to get through ~100 such tests in a couple hours at the Swipely hackfest (while also watching movies, drinking beers, and joking around), and each one of which taught me something new about the Scala language.  Within the weekend, I was able to finish the rest of the Koans (total of 276 currently), and felt like I finally had a bit of real appreciation for the types of problems it might solve better than Ruby (more on this later).

Not only did I start learning Scala, but I discovered a teaching method that really impressed me.  Imagine if every software project had a similar koan suite.  New developers that worked through the koans would not only learn the codebase, but they would develop the beginnings of a strong TDD workflow.  In my experience, both of these things are hard to teach and extremely valuable.

## Play!

After finishing the koans, I did some more-informed searching.  I was now able to appreciate that the [Play! framework](http://www.playframework.org/), while less popular than Lift, might be a better fit for my goals and experience.  I built the [demo app](http://www.playframework.org/documentation/2.0.4/ScalaTodoList) and deployed it to Heroku within an hour of starting.  This was possible both because the framework has strong similarities to Rails, and because the tutorial documentation is extremely easy to follow.  Any Rails developer who wants to deploy a Scala app as soon as possible should start here (but then do the Koans, or else you'll just be writing Ruby in Scala).

## Next Steps

Further research suggests that [the Akka library](http://akka.io/) would be a good choice to learn next.  The actor model seems to play to Scala's strengths.  I have a hobby project that needs some realtime communication, so once I feel comfortable with Akka, I see no reason not to start implementing the back-end for that project using what I've learned.

That said, I'm extremely open to advice from more experienced Scalaists.  Please get at me at [@mattgillooly](http://twitter.com/mattgillooly) if you have something to add!
