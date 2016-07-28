# Messaging

This is a Working Draft of the Intent, Scope, Concepts, Specification, and Components of Messaging (working name TBD).


## History

We (@subramaniank, @sandeep4 and I) have worked on messaging for the last year at MagicTiger and later MagicX.

Over the course of the past year, we've had to put in a number of hacks to make messaging just work.

We'll use the lessons learnt as a starting point here.


## Intent

With the advent of bots, messaging is becoming a central piece of the software we write.

Through the past year, we often found ourselves hacking together and re-purposing parts of older software to get our job done.

With the rise of bi-directional messaging and conversational UI on chat and web, the need for a new breed of frameworks has become apparent.

Through our components, we aim to provide smaller composable units that can be used to make such frameworks possible.

Sample implementations will be covered by various tutorials over time.

## Terms

**Component:** A component is a logical unit of composable and independently scaling unit in the architecture.
In some cases the term *component* is synonymous with a microservice, in others another open source project could be dropped in with a thin wrapper. This document deliberately avoid those terms to keep the concepts separate from implementation.

(TK)

## Components

* Socket manager / API gateway

* Message Buffer / Queues

* Exchange / Routing

* Persistence

* State Manager
