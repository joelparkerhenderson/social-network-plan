# Topologies: centralize, decentralize, distribute, federate?

[Issue discussion](https://github.com/joelparkerhenderson/social_network_plan/issues/12)

Discuss potential topologies of the social network, such as whether it is essentially centralized (as are Facebook and Twitter) or decentralized/distributed/federated (as are Mastodon and Secure Scuttlebutt).


### Quotations

Quotations to consider:

* "The only way social is going to work and be improved going forward is through decentralisation and taking our data out of the hands of a central repository where it can be used to target us, and is more vulnerable to breaches. Once we have that baseline the other problems can be solved by the communities themselves."

* "The web that many connected to years ago is not what new users will find today. The fact that power is concentrated among so few companies has made it possible to weaponize the web at scale."

* "The whole issue with the first decentralised networks at the moment are their usability and accessibility to the average person. There’s a lot of work to be done on this. There are 1000s of people tackling the problem globally from the protocol level to the user interfaces."


* "Social protocols are the answer. They probably won't be the first answer. You need some of these networks with real traction (or at least one huge one) so they can derive a protocol from the greatest common factors between them. To preemptively make a protocol sans popular implementation has little value and often ends in low adoption. As we've learned, the success of a protocol is more about its popularity than its presence or quality. So I say let these networks gestate and once the market (of people, not money) starts picking winners, then begin your abstraction. And for those (of us) working on solutions to this problem space now, keep going. You don't need a committee or standards doc or whatever. You just need an awesome implementation."

* "On a distributed network you replicate data only with people you choose. Since you're not going to add a government (or an ad company) to your friend list, they won't have your data. Private communications are encrypted and flowing directly to the recipient, so there's no port that agencies can tap into to listen. There won't be any big data to analyze, since data is spread across the network. Backup is easy, it's just a folder. Fake news never gets promoted, since there are no paid promotions. Spam is a non-issue since there are no advertisers. There's no way to get into your feed than through your friends. There's no server or central storage, so employee misuse is not an issue. And you can have as many identities as you choose, there won't be a mandatory real name policy."

* "Facebook is centralized. Diaspora is federated; the individual nodes (to which thousands of users are connected) will have far fewer resources to secure themselves than a behemoth like FaceBook, and also have issues of uptime, badwidth, etc. ScuttleButt is peer to peer, somewhat like torrents but for data feeds; more specifically, it's partially peer to peer because it uses gossip, so at times your peer might be a semi-centralized server, and at other times it could be a peer."


### Wordbook

Wordbook of terminology:

* [Distributed social network - Wikipedia](https://en.wikipedia.org/wiki/Distributed_social_network)
* [Distributed Social Networks - P2P Foundation](https://wiki.p2pfoundation.net/Distributed_Social_Network_Projects)


### Commentary

* [Thoughts on federated social networks - by Matt Lee](https://medium.com/@mattl/thoughts-on-federated-social-networks-9f2962481911)
* [Scuttlebutt, a decentralized alternative to Facebook](https://www.inthemesh.com/archive/secure-scuttlebutt-facebook-alternative/)
* [Decentralized social networks sound great - too bad they'll never work - by Wired)](https://www.wired.com/story/decentralized-social-networks-sound-great-too-bad-theyll-never-work/)


## Considerations

Do distributed social networks exacerbate the problems that Facebook has been seeing so much backlash against?


### Exploits

The Facebook Cambridge Analytica issue was caused by APIs that are too open. 

For distributed systems, are there more ways to exploit the APIs and gather data on users?

Some technologies believe that distributed systems can use more-protectable protocols and more-protectable encryption. 

Comments:

* "Scuttlebutt is "fully encrypted", and thus the API is more locked down than Facebook/etc."

* "Scuttlebutt is not at all "fully encrypted", and it's fairly trivial to spider and download just about everything; the hardest part is the first foothold (which can be found posted various places, including the official docs on ssb), from there, downloading the entire "social web" it has can be done with the "main client" by basically changing a single config value."

* "Scuttlebutt is not "fully encrypted" as is, yet can use point-to-point encryption between nodes, and can also be optionally extended to use public-private keys for exchanging secure messages."

* "TOR is fully encrypted, but there are somewhat regular vulnerability reports about various parts of the stack. Including criticial vulnerabilities that can and have been exploited by nation states, for example."

* "The attack surface for Scuttlebutt is much larger than for Facebook, and I trust Facebook's security team to audit and patch much more than I trust any random friend."


### Accountability

There is a clear issue with Facebook's accountability. 

Distributed run on multiple servers, with multiple owners, and may also be open source.

Does this lead to any areas of zero accountability?

Comments:

* "If I had a magic wand, I'd solve this by splitting Facebook into an infrastructure-and-core-data non-profit and one or more for-profit companies that are building tools or interfaces on that platform."

* "I think there is a natural monopoly for some aspects of this, which is why Facebook is so hard to quit. But I don't think the whole thing need be in private, for-profit hands. Mozilla shows that a nonprofit can be a good steward of important web assets, with much stronger user advocacy than for-profit companies normally do. Doing something like that for identity and interconnect between messaging and micropublishing providers seems much more robust than pure decentralization to me, which I expect would have the same failure mode as OpenSocial [1], where forces pushing toward natural monopoly are basically unchecked."


### GDPR

How does a distributed system do GDPR compliance?

Comments:

* "A distributed social network is in a worse position than Facebook because there's no one to have responsibility to be accountable. As far as I know it doesn't matter if you're a person or a company, if you're collecting data, it's something you can be liable for. So in a distributed system, all parties who maintain the data sources would be liable."

* "As far as GDPR goes, you're right that a distributed network has different issues, because you're specifically choosing people to send your messages to. However, having a mechanism to delete your messages on other people's systems when they sync would probably go a long way."

* "The GDPR argument is a bit moot because Scuttlebutt is no different than sharing pictures in gossip style (a.k.a. memes). If one of your childhood pictures happens to become the new meme, there's little hope that GDPR enforcement would suffice to de facto delete it from the internet: from Reddit, from Imgur, from independent websites, from Torrent, etc. The same is with Scuttlebutt, but data is primarily shared between friends without contracts, not from people to a particular company. GDPR applies to institutions."


### Login

Comments:

* "A lot of people like using Facebook as a login system. Maybe WebAuthn will help with that since it’s a valid use but most people didn’t see what else they were agreeing to."


### Usability

Some of the problems with Facebook are more about usability and clarifying how things work to users, for instance the scandal with people giving away access to their private messages.

Open source software and distributed software tends to be much harder to use.

How to make an open source and/or distributed social network easier to sue?


### Future-proofing

Will any future concern/issue be harder to resolve if there are many different instances running decentralized social networks?


### Security

Using AI to detect abusive content or spot fake news is much harder if you only have a subset of the data. 

Does it becomes harder to address these concerns in a distributed setting?

Comments:

* "In a decentralized world, there's no one who has access to holistically examine automated access and detect shady activity. In a decentralized world, everything is essentially a third-party app.""


### Policies

Comments:

* "We fail to consider policy when thinking about centralized/federated services. Centralized services provide strong, regular policy adherence across the network, whereas federated services provide weak, irregular policy adherence across the network. Centralized services can effectively silence a bad actor. They may also silence a good actor, but generally only under external pressure from government. Federated services have little or not ability to silence bad actors across the network, though individual instances may effectively silence "bad" actors. However in this capacity "bad" is not well understood and can simply mean the instance administrator does not like the person the silence. Individual instances may also give voice to bad actors."


### Notifications

Comments:

* "I’ve seen a lot of people use are notifications / invites. e.g. most big gaming communities are bad experiences but you can bootstrap your friends into a better group. That seems harder to change and it’s definitely a real need.



