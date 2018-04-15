# Social Network Plan

Work in progress notes about how to build a social network for social good.

* [Introduction](#introduction)
  * [Abstract](#abstract)
  * [Feedback](#feedback)
  * [About this document](#about-this-document)
* [Baseline](#baseline)
  * [Social context](#social-context)
  * [Technical context](#technical-context)
* [Challenges](#challenges)
  * [Open issues](#open-issues)
  * [How to describe a social network?](#how-to-describe-a-social-network-)
  * [Articles](#articles)
* [Minimum Viable Product](#minimum-viable-product)
  * [Yes, likely in scope](#yes-likely-in-scope)
  * [Maybe, possibly in scope](#maybe-possibly-in-scope)
  * [No, not in scope](#no-not-in-scope)
* [User Experience](#user-experience)
  * [Sign in](#sign-in)
  * [Stories](#stories)
  * [Routes and meta-routes](#routes-and-meta-routes)
* [Implementation](#implementation)
  * [Planning](#planning)
  * [Full stack](#full-stack)


## Introduction


### Abstract

Social networks such as Facebook and Twitter enable people to connect with each other, share messages, and publish media. 

We believe social networks have significant benefits for people and society. However, we also believe that the big social networks suffer from major problems: data breaches, fake accounts, poor accountability, rife advertising, and restricted rights; these problems harm people and society. 

We propose a social network plan that is not-for-profit (NFP), uses free/open/libre source (FLOSS), and is for social good.


### Feedback

We welcome feedback, suggestions, and constructive criticism. Email joel@joelparkerhenderson.com, tweet ([@joel_henderson](https://twitter.com/joel_henderson)), or comment in our [issues](https://github.com/joelparkerhenderson/social_network_plan/issues).


### About this document

This is a work in progress and will improve as we learn. 

We want this document to be a friendly introduction, rather than a comprehensive reference, or societal manifesto, or technical specification. 

We want to explore the viability of new social network for social good. We want to explore the purpose i.e. why do this, and the pragmatics i.e. how to do this.

We use quotations with light editing for content, context, readability, consistency, and anonymity.


## Baseline


### Social context

We are looking at the biggest social networks such as 
[Facebook](https://facebook.com) and
[Twitter](https://twitter.com).

We like websites using technology for social common good such as 
[Wikipedia](https://wikipedia.org) and
[Craigslist](https://craigslist.org).

We look to technology advocacy groups such as 
[Electronic Frontier Foundation (EFF)](http://eff.org/) and
[Open Source Initiative (OSI)](http://https://opensource.org/).


### Technical context

We are frequent users of social coding sites such as 
[GitHub](https://github.com) and
[StackOverflow](https://stackoverflow.com).

We are users of social identity tools such as 
[GPG](https://www.gnupg.org/) and
[Keybase](keybase.io).

We like decentralized distributed social networks such as
[Mastodon](https://mastodon.social) and
[Patchwork](https://github.com/ssbc/patchwork).


## Challenges


### Open issues

Open issues that are especially important to discuss:

* [**Funding**: advertisements, donations, subscriptions?](https://github.com/joelparkerhenderson/social_network_plan/issues/1)
* [**Audience**: general public, niche groups, special needs?](https://github.com/joelparkerhenderson/social_network_plan/issues/2)
* [**Scope**: benefits, features, minimum viable product?](https://github.com/joelparkerhenderson/social_network_plan/issues/3)
* [**Comparisons**: similarities/differences versus others?](https://github.com/joelparkerhenderson/social_network_plan/issues/4)
* [**Names**: real names, fake names, no names?](https://github.com/joelparkerhenderson/social_network_plan/issues/5)
* [**Data**: who owns it, who uses it, who controls it?](https://github.com/joelparkerhenderson/social_network_plan/issues/6)
* [**Security**: spammers, hackers, masqueraders?](https://github.com/joelparkerhenderson/social_network_plan/issues/7)
* [**Community**: how can we encourage people to help?](https://github.com/joelparkerhenderson/social_network_plan/issues/8)
* [**Motivation**: gamification, extrinsic, intrinsic?](https://github.com/joelparkerhenderson/social_network_plan/issues/9)
* [**Niches**: music, meets, malls, mashups, more?](https://github.com/joelparkerhenderson/social_network_plan/issues/10)
* [**Feeds**: linear, algorithmic, customizable?](https://github.com/joelparkerhenderson/social_network_plan/issues/11)
* [**Topology**: centralized, decentralized, distributed, federated?](https://github.com/joelparkerhenderson/social_network_plan/issues/12)
* (more?)

<!--
Original content vs. resharing

* "Reshares are part and parcel of a community - even before the days of the Internet. For many, gossip is part of socializing. A friend posted that he's just getting married. People will want to spread the word. How can they without reshares? Rewrite it themselves? Resharing is simply part of usual human interaction."
-->


### How to describe a social network?

We see challenges in how people describe social networks; we suggest starter questions.

Examples:

* **Benefits**: give me reasons to try your product.
* **Privacy**: what is your privacy policy, including sharing with 3rd party?
* **Platform**: is your product aiming to be a platform, API, plugin, integation, etc.?
* **Access**: mobile, web, desktop, native, etc.?
* **Code**: open source, closed source, etc.?
* (more?)


### Articles

We are reading articles and posts by social network advocates such as:
* [Social media and its discontents by Cal Newport](http://calnewport.com/blog/2018/03/20/on-social-media-and-its-discontents/)
* [Paradigm shifts for the decentralized web](https://ruben.verborgh.org/blog/2017/12/20/paradigm-shifts-for-the-decentralized-web/)
* [The Search for the Anti-Facebook](http://www.slate.com/articles/technology/future_tense/2014/10/ello_diaspora_and_the_anti_facebook_why_alternative_social_networks_can.html)
* [Let's verify real people, not real names](https://bford.github.io/2015/10/07/names.html)
* [Y Combinator’s nonprofit funding](https://blog.ycombinator.com/what-y-combinator-looks-for-in-nonprofits/)
* [Human Connection](https://human-connection.org)
* (more?)


## Minimum Viable Product

We believe that to be successful, the best path is to create the simplest-possible social network that people will actually use. This is a minimum viable product (MVP).


### Yes, likely in scope

Capabilities that we believe must be in scope:
* Join: e.g. sign up, sign in, sign out, manage your data, delete your account
* Post: e.g. with a combination of title, text, link, image
* Wall: e.g. a profile page, news feed, timeline, calendar
* Item: e.g. a person, place, event, organization


### Maybe, possibly in scope

Capabilities that we like, yet don't know if they must be in scope:
* Mark: e.g. like, love, star, upvote, downvote, flag, tag
* Blob: e.g. photo, video, audio, document
* Team: e.g. group, circle, room, forum, channel, categories
* Chat: e.g. comment, message, mail


### No, not in scope

Capabilities that we want to defer to future scope:
* Mobile apps
* Old browsers
* Live streams
* Notifications
* Payments


## User Experience


### Sign in

Discuss sign in options via:
* Email address and password
* Multi-factor e.g. mobile phone SMS, Google Authenticator app
* Providers e.g. Google, Facebook, LinkedIn
* Protocols e.g. OAuth, SAML
* Integrators e.g. Okta.com


### Stories

Discuss stories:
* Can we use RSS?
* Can we use Atom?
* Why/how to provide what companies say they want, e.g. ads, analytics, branding?


### Routes and meta-routes

We use the term "route" to generically describe a way to reach people, places, items, etc.

Examples:

* Email addresses: <a href="mailto:alice@example.com">alice@example.com</a>
* Phone number: <a href="tel:1-415-317-2700">1-415-317-2700</a>
* Website page: <a href="http://reddit.com">http://reddit.com</a>

We use the term "meta-route" to generically describe a route that contains another route. 

Examples where each website URL route contains another route:

* Email address: <a href="https://www.example.com/alice@example.com">https://www.example.com/alice@example.com</a>
* Phone number: <a href="https://www.example.com/1-415-317-2700">https://www.example.com/1-415-317-2700</a>
* Website page: <a href="https://example.com/reddit.com">https://example.com/reddit.com</a>

Brainstorms:
* We speculate that meta-routes may make it easier, faster, and better, to create a user-friendly social network that also connects to other networks.
* For example meta-routes can automatically give each person their own page based on their email address, or on their multiple email addresses; the person doesn't have to choose a new username or compete with other people for usernames.
* For example, meta-routes may improve people's trust in the network, because the URL contains more information that can be automatically verified, such as verifying the person's email address by sending an email, or telephone number by sending a text message, or website page by having a webmaster add a page identifier.


## Implementation


### Planning

Discuss broad goals:
* This project is more akin to an ambitious web app, less akin to a blogging site.
* We value participation by many people and organizations.
* The security needs to be bulletproof and independently-verifiable.

Discuss organizational areas:
* Prefer truly free technology over corporate-restricted technology.
* Prefer more-welcoming communities over less-welcoming communities.
* Prefer agile over waterfall.

Discuss project management such as:
* Planning e.g. Asana, Trello
* Dicussion e.g. IRC, Slack
* Prototyping e.g. Balsamiq, Photoshop

Discuss planning methodologies:
* Agile, lean, kanban, waterfall, etc.
* Model, view, controller (MVC), data, context, interaction (DCI), etc. 
* Functional code may be easier to create reliably and easier to scale up.


### Full stack

Discuss languages such as:
* Popular tech e.g. React, Node, C++
* Powerful tech e.g. Java, Kotlin, Clojure
* Progressive tech e.g. Ember, Elixir, Rust
* Mobile tech e.g. iOS, Android, React Native

Discuss databases such as:
* Relation-oriented e.g. MySQL, PostgreSQL, SQL Server
* Document-oriented e.g. Mongo
* Speed-oriented e.g. Redis, Memcached
* Graph-oriented e.g. Fauna, Neo4J
* Vendor-oriented e.g. Google Spanner, Amazon Aurora

Discuss data exchange such as:
* Resource-oriented e.g. REST-like
* Graph-oriented e.g. GraphQL-like
* Object-oriented e.g. RPC
* Wire-oriented e.g. protocol buffers, thrift
* Publishing-oriented e.g. RSS, Atom, Pub/Sub
* API-oriented e.g. JSON API, OpenAPI, LD, RDF, SPARQL

Discuss platform areas such as:
* Mobile vs. desktop
* Phone size vs. tablet size vs. laptop size
* Distribution on Windows, Mac, Linux, iOS, Android, etc.
* Distribution via Apple App Store, Google Play, etc.


