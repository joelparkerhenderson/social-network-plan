# Names: real names, fake names, no names?

[Issue discussion](https://github.com/joelparkerhenderson/social_network_plan/issues/5)

Discuss names, such as whether a user should be required to use their real name, or can optionally use a fake name or pseudonym, or can optionally use an anonymous name such as a random token.


### Quotations

Quotations to consider:

* "We want people to know who they are connecting to, and we want you to have an authentic experience. So we require you to use your real name, as it would be listed on your credit card, government ID, workplace ID, or student ID."

* "Some people like to use fake names and pseudonyms. These are good for established alter-egos, such as people with pen names. These are also good for people who may need to protect themselves because they may be targets of persecution."

* "Real name policies are unreliable, impossible to enforce correctly, and disproportionally cause problems for ethnic groups and people with unusual names, multiple names, or cross-cultural names."


### Facebook and real names and numbers

See https://news.ycombinator.com/item?id=18727230

Facebook has (inadvertently) pulled off the most stunning type of misdirection about the real competitive advantage of Facebook. Programmers are mislead into looking at one thing (e.g. "personal websites") when they really should be looking at something else: The Real Names Lookup Database. The Real Names Lookup Database is what makes the other features such as "point-to-point messaging", "chat", "calendar events", and finally "personal blog platform" aka "personal websites" -- all work so well with minimum friction.

If you still have doubts whether Facebook's special sauce is the real_names database or if it's the "ease of personal websites", consider what Facebook chooses to spend billions on: Instagram ($1 billion), WhatsApp ($19 billion), and attempt to acquire Snapchat ($3 billion). Facebook does not bother with acquiring "easy-to-use website builders" such as Wix, or Squarespace. What do Instagram/WhatsApp/Snapchat have in common that Wix/Squarespace do not? A database of real phone numbers of their users.

On a related note, thinking that a protocol like ActivityPub can replace Facebook is also misguided analysis. ActivityPub is not a "real names lookup database" so it can't replace the actual thing that makes Facebook useful. Instead of focusing on protocols, think of how to make an alternative database of real-names-lookup that isn't owned by Facebook. Also think of where the database will be physically stored (blockchain is probably not the answer), and how costs for the maintenance of the database will be paid.

Without a viable real_names lookup database, it's pointless for Everybody To Have Personal Websites because there's no easy way for them to connect to other relevant websites to share data. That "connection" is easiest and more scalable when it's based on real names instead of urls.

For a database lookup of domain names to ip addresses, we have a canonical and universal "database": DNS. It's also very useful to have a "real names" reverse-lookup to "web profiles" but right now, the closest analogy we have to that is the realnames database privately owned by Facebook.

Facebook themselves took roughly 10 years to build it, and they used a lot of psychological tricks to do it (first mover advantage, early FB was "exotic" and "invite only", late FB was an avalanche of FOMO and network effects, etc). Similarly, the history of the White Pages and the Yellow Pages is a fascinating read and took decades for those books to be accepted.
