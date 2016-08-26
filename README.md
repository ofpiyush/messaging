# Messaging

This is a Working Draft of the Intent, Scope, Concepts, Specification, and Components of Messaging (working name TBD).


## History

We ([@subramaniank](https://github.com/subramaniank), [@sandeep4](https://github.com/Sandeep4) and [@ofpiyush](https://github.com/ofpiyush)) have worked on messaging for the last year at MagicTiger and later MagicX.

Over the course of the past year, we've had to put in a number of hacks to make messaging work.

We'll use the lessons learnt as a starting point here.


## Intent

With the advent of bots, messaging is becoming a central piece of the software we write.

Through the past year, we often found ourselves hacking together and re-purposing parts of older software to get our job done.

With the rise of bi-directional messaging and conversational UI on chat and web, the need for a new breed of frameworks has become apparent.

Through our components, we aim to provide smaller composable units that can be used to make such frameworks possible.

Sample implementations will be covered by various tutorials over time.

## Definitions

**Component:** A component is a logical unit of composable and independently scalable architecture.
In some cases the term *component* is synonymous with a microservice, in others another open source project could be dropped in with a thin wrapper. This document deliberately avoids those terms to keep concepts separate from implementation.

**Client:** A client is a uniquely identifiable user of this system. It is important to note the distinction between a client and a single connection.

Eg: A client can be a human with their app/web on a single connection or a third party service with multiple horizontally scalable instances connecting with the same *identity*.

**Vendor:** A vendor of the system is an identity with access to a group of clients.

(TK)

## Components

* [Connection manager (Socket / HTTP)](./ConnectionManager.md)

* Message Buffer (Inbox / Queues)

* [Backend (Exchange / Routing / Web Server)](./Backend.md)

* Persistence (logging / long term data store)

* State Manager ( user sessions / presence / roster)
