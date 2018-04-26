# Secure Scuttlebutt (SSB)

Secure Scuttlebutt is a newer protocol for exchanging information, essentially as a peer-to-peer append-only tamper-proof log.

See https://github.com/ssbc/secure-scuttlebutt

This page is for discussion questions.


### Best uses

What are areas where SSB can shine, and that are also very hard to do without SSB?

Use case idea: disaster relief, such as first-responder networks when there's no WiFi and no mobile phone service. (This is the actual use case of one of my friend's projects)

Use case idea: a population center is attacked by military, and all typical comms for civilians are broken or surveilled; people flee into the hills and into caves, for many months. (This is the actual use case of my current project)


### Single identity, multiple feeds

How does someone create multiple feeds and associate them?

Use case idea: I want to publish one feed for friends and one feed for coworkers.

Use case idea: a company wants to publish a feed per product.


### Corrections

What happens if a user posts information then wants to change it?

Use case: I accidentally publish a broken link, and I want to publish the correct link.

What's the recommended way to do a correction and/or revocation and/or to supersede an earlier item?

Does it make any difference if my system has connected to another system (i.e. the broken link item was shared with another SSB) or not (i.e. the broken link item never left my system).


### Deletions

Use case: I publish thousands of items, and years later I want to delete an old item.

I'm seeking answers beyond "SSB doesn't do that" or "There's no way for a user to control the data once its broadcast"; I'm seeking an answer that speaks to real world needs for serious risks including victim protection.


### Supersede/revoke

What happens if a user posts information that must be wiped?

Use case: I accidentally publish a broken link, and the first person who reads my post tells me, so I want to correct it ASAP by publishing a new link that supersedes the broken link.

Use case: I publish thousands of items, and years later I want to delete an old item.

I'm seeking answers beyond "SSB doesn't do that" or "There's no way for a user to control the data once its broadcast"; I'm seeking an answer that speaks to real world needs ranging from as a novice accidentally publishing something in error, or an expert wanting to excise history for purposes of victim protection.


### Load testing

What approaches could be relevant for load testing?

Use case idea: I follow ~1000 accounts, have ~1000 followers, and everyone posts ~1 daily.


### Keyframes

What approaches could be relevant for creating keyframes, or saltatory conduction, or waypoints, etc.?

Use case: a chain has 1M messages, stretching back years, and I want soley today's news.


### Encryption everywhere

For the sake of argument, assume that the Internet continues its decades-long pattern of moving toward encryption everywhere, e.g. hiding content by changing from telnet to SSH, from FTP to SFTP, from HTTP to HTTPS, etc.; what's involved and what changes if SSB goes toward encryption everywhere?

Use case idea: I want to have a private invitation-only feed for my coworkers, and I prefer to know that all content we exchange uses encryption everywhere, ideally when in motion and also at rest.


### Disposable sub-keys

If my keys are breached, what do I do?

Use case idea: I use a GPG master key on an air-gapped Thinkpad with a specific CPU that I want, and I use the GPG master key to generate disposable sub-keys; I keep all my original content, so if/when a sub-key is breached, then am able to revoke the sub-key, then sign the original content with a new sub-key; how does SSB approach this kind of updating?


### Single-purpose security

SSB uses the public key as the sole public identifier. There is a general purpose security concept that it's wiser to use an item for one purpose only, e.g. use the item as a key or an identity, but not both. What is your team's position on this?

Use case idea: my intuition is it's better to have a separation of concerns, for example I prefer to unlock my phone with a passcode (i.e. single purpose) rather than with my fingerprints (i.e. because my fingerprints are my identity elsewhere, and also are also near-impossible to change).


