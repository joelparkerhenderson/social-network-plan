# Social Network Plan

Work in progress notes about how to build a social network for social good.

* [Introduction](#introduction)
  * [Abstract](#abstract)
  * [About](#about)
  * [Context](#context)
* [Challenges](#challenges)
  * [Open issues](#open-issues)
  * [How to describe a social network?](#how-to-describe-a-social-network-)
* [User Experience](#user-experience)
  * [Sign in](#sign-in)
  * [Stories](#stories)
* [Implementation](#implementation)
  * [Planning](#planning)


## Introduction


### Abstract

We believe social networks have significant benefits for people and society. However, the big social networks suffer from major problems: data breaches, fake accounts, poor accountability, rife advertising, and restricted rights; these problems harm people and society. We propose a social network plan that aims for social good, as a not-for-profit (NFP), using free/libre open source (FLOSS).

### About

Goal:
* We want to explore the viability of new social network for social good. 
* We want to explore the purpose i.e. why do this, and the pragmatics i.e. how to do this.

Scope:
* We want this to be a friendly introduction that invites discussion.
* We do not want this to be a reference, or manifesto, or specification. 

Feedback:
* We welcome feedback, suggestions, and constructive criticism. 
* Email joel@joelparkerhenderson.com, tweet [@joel_henderson](https://twitter.com/joel_henderson), or comment in our [issues](https://github.com/joelparkerhenderson/social_network_plan/issues).

Updates:
* This plan is a work in progress, and likely to change as we learn more. 
* We are actively making requests for comments, and we add these as we go.

Quotations:
* We use quotations with light editing for content, context, readability, consistency, and anonymity.


### Context

Overview:
* We are looking at the biggest social networks such as 
[Facebook](https://facebook.com),
[Twitter](https://twitter.com),
[LinkedIn](https://linkedin.com).
* We like websites that use technology for social good such as 
[Wikipedia](https://wikipedia.org),
[Craigslist](https://craigslist.org),
[Archive.org](https://archive.org).

Advocacy:
* We look to foundations such as 
[Electronic Frontier Foundation (EFF)](http://eff.org/) and
[Free Software Foundation (FSF)](http://fsf.org).
* We look to FLOSS groups such as 
[Open Source Initiative (OSI)](http://opensource.org/) and 
[Software Freedom Conservancy (SFC)](https://sfconservancy.org/).

Technology:
* We use social coding sites such as 
[GitHub](https://github.com) and
[StackOverflow](https://stackoverflow.com).
* We use social identity tools such as 
[GPG](https://www.gnupg.org/) and
[Keybase](keybase.io).
* We admire distributed social networks such as
[Mastodon](https://mastodon.social) and
[Patchwork](https://github.com/ssbc/patchwork).


## Challenges


### Open issues

Open issues that are especially important to discuss:

* [**Funding**: advertisements, donations, subscriptions?](docs/funding.md)
* [**Audiences**: general public, niche groups, special needs?](docs/audiences.md)
* [**Scopes**: benefits, features, minimum viable product?](docs/scopes.md)
* [**Comparisons**: similarities/differences versus others?](docs/comparisons.md)
* [**Names**: real names, fake names, no names?](docs/names.md)
* [**Data**: who owns it, who uses it, who controls it?](docs/data.md)
* [**Security**: spammers, hackers, masqueraders?](docs/security.md)
* [**Communities**: how can we encourage people to help?](docs/communities.md)
* [**Motivations**: gamification, extrinsic, intrinsic?](docs/motivations.md)
* [**Niches**: music, meets, malls, mashups, more?](docs/niches.md)
* [**Feeds**: linear, algorithmic, customizable?](docs/feeds.md)
* [**Topologies**: centralized, decentralized, distributed, federated?](docs/topologies.md)
* [**Routes**: how to reach people, places, items, resources?](docs/routes.md)
* [**Stacks**: languages, frameworks, databases, interfaces, etc.?](docs/stacks.md)
* [**References**: articles, blogs, commentaries, etc.?](docs/references.md)

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
