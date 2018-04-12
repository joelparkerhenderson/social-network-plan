# Social Network Plan

Work in progress notes about how to build a social network for social good.

* [Introduction](#introduction)
  * [Abstract](#abstract)
  * [About this document](#about-this-document)
  * [Baseline](#baseline)
  * [Challenges](#challenges)
* [Debates](#debates)
  * [Social internet vs. social media](#social-internet-vs-social-media)
  * [Subscriptions vs. free](#subscriptions-vs-free)
  * [Ranked feed vs. linear feed](#ranked-feed-vs-linear-feed)
  * [Original content vs. resharing](#original-content-vs-resharing)
  * [External motivation vs. intrinsic motivation](#external-motivation-vs-intrinsic-motivation)
  * [Centralized vs. decentralized](#centralized-vs-decentralized)
  * [Mobile vs. desktop](#mobile-vs-desktop)
* [Minimum Viable Product](#minimum-viable-product)
  * [Capabilities](#capabilities)
  * [Niche ideas](#niche-ideas)
  * [Differentiation ideas](#differentiation-ideas)
* [User Experience](#user-experience)
  * [Sign in](#sign-in)
  * [Stories](#stories)
  * [Routes](#routes)
* [Technical Implementation](#technical-implementation)
  * [Working assumptions](#working-assumptions)
  * [Languages](#languages)
  * [Databases](#databases)
  * [Data exchange](#data-exchange)
  * [Project management](#project-management)


## Introduction


### Abstract

Social network sites such as Facebook and Twitter these social sites enable people to connect with each other, to share messages and media, and stay informed. We believe social network sites have many significant benefits for people and for society. 

However, we also believe that some social networks are growing out of control, beholden to special interests such as financiers and user data aggregation advertisers, and that these special interests are significantly dangerous to people and to society. 

We therefore propose new social network ideas for community discussion, such as a social network that is a not-for-profit (NFP), a social network that uses free/open/libre source (FLOSS), and a social network that is founded on social good.


### About this document

We are using this document a work in progress. We are improving this document as we learn. 

We welcome suggestions, feedback, advice, ideas, and constructive criticism. You can contact us by email (joel@joelparkerhenderson.com), Twitter (@joel_henderson), or by using GitHub issues or pull requests.

We intend this document to be a friendly introduction to the areas that we want to discuss; we do not intend for this document to be a comprehensive reference, or a literature review, or a societal manifesto, or a technological specification. We do welcome links to all these areas.

We want to use this document to explore the viability of new social network that helps people. Specifically, we want this document to look at both the purpose i.e. why do this, and also the pragmatics i.e. how to create this.

We use quotations with light editing for content, context, readability, consistency, and anonymity.



### Baseline

We are looking at the biggest social networks.

Prominent examples:

* [Facebook](https://facebook.com)
* [Twitter](https://twitter.com)
* [LinkedIn](https://linkedin.com)
* (more?)

We are inspired by initiatives that use websites and technology toward common good. 

Prominent examples:

* [Wikimedia Foundation - Wikipedia.org](https://wikimediafoundation.org)
* [Internet Archive - Archive.org](https://archive.org)
* [Y Combinator’s nonprofit funding](https://blog.ycombinator.com/what-y-combinator-looks-for-in-nonprofits/)
* [Human Connection](https://human-connection.org)
* (more?)

We are learning about newer kinds of technologies such as distributed social networks. 

Prominent examples:

* [Diaspora](https://diasporafoundation.org/)
* [Mastodon](https://mastodon.social)
* [Patchwork on Secure Scuttlebutt (SSB)](https://github.com/ssbc/patchwork)
* (more?)

We are researching position posts by advocacy leaders.

Prominent examples:

* [Social media and its discontents by Cal Newport](http://calnewport.com/blog/2018/03/20/on-social-media-and-its-discontents/)
* [Paradigm shifts for the decentralized web](https://ruben.verborgh.org/blog/2017/12/20/paradigm-shifts-for-the-decentralized-web/)
* [The Search for the Anti-Facebook](http://www.slate.com/articles/technology/future_tense/2014/10/ello_diaspora_and_the_anti_facebook_why_alternative_social_networks_can.html)
* (more?)

We are frequent users of social coding sites.

Prominent examples:

* [GitHub](https://github.com)
* [Bitbucket](https://bitbucket.org)
* [StackOverflow](https://stackoverflow.com)
* (more?)

We are users of social identity tools.

Prominent examples:

* [GPG: The GNU Privacy Guard](https://www.gnupg.org/)
* [Keybase](keybase.io)
* (more?)

We donate to technology groups that may be relevant:

* [Apache Software Foundation (ASF)](http://apache.org/)
* [Electronic Frontier Foundation (EFF)](http://eff.org/)
* [Free Software Foundation (FSF)](http://www.fsf.org/)
* [Linux Foundation](http://www.linuxfoundation.org/)
* [Open Source Initiative (OSI)](http://https://opensource.org/)
* [Software Freedom Conservancy](https://sfconservancy.org/)


### Challenges

We see challenges in how people describe social networks; we suggest starter questions.

Examples:

* Benefits: give me reasons to try your product.
* Differentiators: how are you different from the incumbents?
* Costs: up-front fee, subscription service, advertising, etc.?
* Audience: are you aiming for a general audience or a specific niche audience?
* Privacy: what is your privacy policy, including sharing with 3rd party?
* Platform: is your product aiming to be a platform, API, plugin, integation, etc.?
* Coordination: centralised, decentralised, federated, etc.?
* Access: mobile, web, desktop, native, etc.?
* Code: open source, closed source, etc.?
* (more?)

We see challenges in significant fundamental areas; we want to research these more.

Prominent examples:

* Identity, such as whether people can use their real names or  pseudonyms.
* Ownership, such as whether people can own their own data and control its sharing.
* Organization, such as how to involve the community, developers, and interest groups.
* Security, such as how to protect from fake accounts, spam messages, and identity theft.
* Funding, such as whether to accept advertising or subscriptions or donations.
* (more?)


## Debates


### Social internet vs. social media

* "Social internet describes the general ways in which the global communication network and open protocols known as “the internet” enable good things like connecting people, spreading information, and supporting expression and activism. Social media, by contrast, describes the attempt to privatize these capabilities by large companies within the newly emerged algorithmic attention economy, a particularly virulent strain of the attention sector that leverages personal data and sophisticated algorithms to ruthlessly siphon users’ cognitive capital."


### Subscriptions vs. advertisements

* "Subscription sounds like it might be a good idea because it seems like it would remove the incentive to monetize personal information, but in practice it creates a barrier to adoption and makes the social network kind of useless."

* "The incentives created by an advertising business model are to essentially addict people psychologically to your product, and then to cause outrage cycles. You want to feed them stuff that either makes them afraid or angry, because when they’re excited by low level emotions like that, they share more stuff, they’re more active, they spend more time on the site, and see more ads, and they’re just more valuable to them."


### General public vs. niche audience

* "The social startups that have struck it big in the post-Facebook era have all started by carving out a different niche. That difference, Cross argues, can’t just be about a site’s back-end architecture or business model, as with Diaspora (an open-source Facebook) or App.net (a Twitter without ads). The product itself has to fulfill a fresh purpose for its users, like sharing snazzy smartphone snapshots (Instagram), networking and advancing their careers (LinkedIn), or showing off their taste in fashion, food, and design (Pinterest)."


### Ranked feed vs. linear feed

* "I wish there was a social network that could somehow avoid people competing to post the highest volume of popular content, so they could relax and focus on posting information about themselves that other people want to know. But even if you were somehow able to force people to just post about themselves, no third-party content, there are plenty of people who would make a meal of it by posting endless videos about their grooming regimen, their cooking, or cute stuff their cat does. It all just devolves into competing for attention."


### Original content vs. resharing

* "Reshares are part and parcel of a community - even before the days of the Internet. For many, gossip is part of socializing. A friend posted that he's just getting married. People will want to spread the word. How can they without reshares? Rewrite it themselves? Resharing is simply part of usual human interaction."


### External motivation vs. intrinsic motivation

* "The more interactions your contributions generate, the more likely you will become a persona leader. Each milestone unlocks rewards, and adds layers of fun to your social connections."

* "The short-term, dopamine-driven feedback loops that we have created are destroying how society works: no civil discourse, no cooperation, misinformation, mistruth."


### Centralized vs. decentralized

* "The only way social is going to work and be improved going forward is through decentralisation and taking our data out of the hands of a central repository where it can be used to target us, and is more vulnerable to breaches. Once we have that baseline the other problems can be solved by the communities themselves."

* "The whole issue with the first decentralised networks at the moment are their usability and accessibility to the average person. There’s a lot of work to be done on this. There are 1000s of people tackling the problem globally from the protocol level to the user interfaces."

* "Social protocols are the answer. They probably won't be the first answer. You need a some of these networks with real traction (or at least one huge one) so they can derive a protocol from the greatest common factors between them. To preemptively make a protocol sans popular implementation has little value and often ends in low adoption. As we've learned, the success of a protocol is more about its popularity than its presence or quality. So I say let these networks gestate and once the market (of people, not money) starts picking winners, then begin your abstraction. And for those (of us) working on solutions to this problem space now, keep going. You don't need a committee or standards doc or whatever. You just need an awesome implementation."


### Mobile vs. desktop

* "I see no compelling reason to be mobile-only at full launch. Mobile-first for your MVP with early adopters, yes that makes a great deal of sense. But when a company does a full launch I think they should support as many of the major platforms as they can (Windows, Mac, Linux, Android, iOS)."


## Minimum Viable Product

We believe that to be successful, the best path is to create the simplest-possible social network that people will actually use. This is a minimum viable product (MVP).


### Capabilities

In scope:
* Join: sign up, sign in, sign out, manage your own data, delete account
* Post: e.g. title, text, link, image
* Wall: e.g. profile page, news feed, timeline, calendar
* Item: e.g. person, place, event, organization

Maybe in scope:
* Vote: e.g. like, love, star, upvote, downvote, flag
* Blob: e.g. photo, video, audio, document
* Team: e.g. group, circle, room, forum, channel

Defer to future scope:
* Chat
* Notifications
* Mobile apps
* Old browsers
* Live streams
* Payments


### Niche ideas

Music ideas:
* Music sharing seems to spread very well e.g. Spotify playlists.
* Music involves many areas e.g. people, bands, clubs, promoters, events, tickets.
* Many people have many opinions and multiple reasons to share.
* Many people love ongoing engagement and also love new discovery.
* Data collection is less risky e.g. data is not medical, business, family.
* Easy to bootstrap e.g. via public data, wikipedia, existing sites.
* Easy to focus geographically on major U.S. cities e.g. LA then NY.

Coupon ideas:
* Coupons are widely understood and have an immediate value prop.
* Coupons are easier to track than ads.
* Coupons involve many areas e.g. people, brands, stores, wallets, redemptions.
* Con: high-end influencers don’t care much about coupons


### Differentiation ideas

Versus Twitter:
* I want a longer username, not limited to 15-characters.
* I want long posts.

Versus Facebook:
* I want separation e.g. peers vs. news, work vs. home, family vs. friends.
* I want a pin area so I can feature my current interests e.g. links to music.
* I want to share with groups of people e.g. circles.
* I want more ways to shape my feed, e.g. more photos of friends, fewer photos of food.
* I want fewer ads and/or more-relevant ads.

Versus LinkedIn:
* I want to be able to apply for jobs more easily.
* I want to feature my skills, rather than feature my resume or CV.
* I want to follow company news, yet not get overwhelmed.
* I want to automatically connect to all my coworkers e.g. enterprise address book.


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


### Routes

Discuss idea of meta-routes using:
* Email address: https://www.example.com/alice@example.com
* Phone number: https://www.example.com/18005551111
* Domain name: https://www.example.com/reddit.com
* Overlay name: https://www.example.com/reddit.com/u/alice
* Key encoding: https://www.example.com/isbn/...
* Geo location: https://www.example.com/map/<lat>,<lng>
* Unique id: https://www.example.com/0x1234567890

Brainstorms:
* Could meta-routes make it easier to sign up?
* Could meta-routes make it much easier to automate account creation?

Overlay site ideas:
* Social: Facebook, LinkedIn, Google+
* Music: Soundcloud, Spotify
* Photos: Imgur, Flickr
* Videos: YouTube, Vimeo
* News: Reddit, Digg


## Technical Implementation


### Working assumptions

Discuss broad goals:
* This project is more akin to an ambitious web app, less akin to a blogging site.
* We value participation by many people and organizations.
* The security needs to be bulletproof and independently-verifiable.

Discuss working assumptions about organizational areas:
* Prefer truly free technology over corporate-restricted technology.
* Prefer more-welcoming communities over less-welcoming communities.
* Prefer agile over waterfall.

Discuss working assumptions about coding methodologies:
* Functional code is easier to create reliably.
* Functional code is easier to scale up on multithreaded machines.



### Languages

Discuss languages such as:
* Popular tech e.g. React, Node, C++
* Powerful tech e.g. Java, Kotlin, Clojure
* Progressive tech e.g. Elm, Elixir, Rust
* Mobile tech e.g. iOS, Android, React Native


### Databases

Discuss databases such as:
* Relation-oriented e.g. MySQL, PostgreSQL, SQL Server
* Document-oriented e.g. Mongo
* Speed-oriented e.g. Redis, Memcached
* Graph-oriented e.g. Fauna, Neo4J
* Vendor-oriented e.g. Google Spanner, Amazon Aurora


### Data exchange

Discuss data exchange such as:
* Resource-oriented e.g. REST-like
* Graph-oriented e.g. GraphQL-like
* Object-oriented e.g. RPC
* Wire-oriented e.g. protocol buffers, thrift
* Publishing-oriented e.g. RSS, Atom, Pub/Sub
* API-oriented e.g. JSON API, OpenAPI, LD, RDF, SPARQL


### Project management

Discuss project management such as:
* Planning e.g. Asana, Trello
* Prototyping e.g. Balsamiq, Photoshop
* Devops e.g. GitHub, CircleCI

