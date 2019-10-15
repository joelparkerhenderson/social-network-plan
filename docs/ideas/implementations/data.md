# Data: who owns it, who uses it, who controls it?

[Issue discussion](https://github.com/joelparkerhenderson/social_network_plan/issues/6)

Discuss data areas, such as who owns data, who uses it and how, who controls it and where it goes?


## Quotations

Quotations to consider:

* "We want to put you in control — and be transparent about what information we have and how it is used."


## References

* [Hard Questions: What Data Does Facebook Collect When I’m Not Using Facebook, and Why?](https://newsroom.fb.com/news/2018/04/data-off-facebook/)


### Data collection

Data collection ideas to consider:

* IP address - can help with routing, langauge localization, etc.

* Browser and operating system information

* The address of the website or app you’re using

* Cookies and device identifiers - can help us determine whether you’re signed in or not

Data collection reasoning:

* IP addresses help us list the countries where people are using an app.

* Browser and operating system information enable us to give developers information about the platforms people use to access their app.

* Cookies and other identifiers help us count the number of unique visitors, and help us recognize which visitors are our users, so we can provide aggregated demographic information, like age and gender, about the people using the site.


## Data for adversting

Data can increase capabilties for advertising-oriented websites and apps to target ads to users.

* When we get a request to show an ad, we need to know where to send it, and the browser and operating system a person is using.

* Cookies and device identifiers help us determine whether the person is our user. If the person is our user, then we can use the fact that they visited a business’s site or app to show them an ad from that business or a similar one. If the person isn't our user, then we can show an ad encouraging them to sign up.

* An advertiser can choose to add our pixel, which is some computer code, to their site. This allows us to give advertisers statistics about how many people are responding to their ads — even if they saw the ad on a different device — without us sharing anyone’s personal information.


## Data for security

Receiving data about the sites a particular browser has visited can help security teams identify bad actors, fault conditions, and malicious payloads.

* Example: if someone tries to log into your account using an IP address from a different country, we might ask some questions to verify it’s you.

* Example: if a browser has visited hundreds of sites in the last five minutes, that’s a sign the device might be a bot. We’ll ask them to prove they’re a real person by completing additional security checks.


## Data for improving offerings

Data can help some websites, apps, and companies, as they aim to improve products and services.

* Example: if you visit a lot of sports sites that use our services, then you might see sports-related stories higher up in your News Feed.

* Example: if you visit a lot of travel sites that use our services, then you might see ads for travel packages, plane flights, and hotels.


## Data controls

We give you a number of controls over the way this data is used to provide more relevant content and ads.

* We require websites and apps who use our tools to tell you they’re collecting and sharing your information with us, and to get your permission to do so.

* News Feed preferences lets you choose which content you see first and hide content you don’t want to see in your feed. You can also view your News Feed chronologically instead of ranked by what Facebook predicts you might be most interested in.

* Ad preferences shows you the advertisers whose ads you might be seeing because you visited their sites or apps. You can remove any of these advertisers to stop seeing their ads.
In addition, you can opt out of these types of ads entirely — so you never see ads on Facebook based on information we have received from other websites and apps.

* If you don’t want us to use your interests to show you ads on other websites and apps, there’s a control for that too.


## Targeting

Reference:

* https://news.ycombinator.com/item?id=16859823

Questions:

* My girlfriend is being shown ads depending on what we do together. How?

* My girlfriend came to check out some open houses with me yesterday after work. By 10 PM, she was seeing ads on Instagram for new houses. She hasn't shopped for a house before, or even done any searches on Google on that topic. I simply invited her to come with me and she did. Similarly, we were at her place the other day and watched a kung fu movie on my laptop (connected to her wifi), and then went to bed. The next morning she started seeing ads for martial arts schools in the area. What is happening?

Answers:

* A totally plausible explanation for this (as plausible as any Amazon Echo passive speech recognition ad targeting theory) is that she's been seeing these ads for weeks, but they were completely irrelevant and her mind filtered them out until she happened to have house hunting / martial arts movies on her mind after these events.

* A possible explanation is cross device targeting using IP address. Most ad tech companies do cross device targeting, using device maps bought from other companies (Drawbridge being one). These companies attempt to assign a variety of devices from the same person to a single advertising profile. The simplest way they do this is by IP address. So if they have an IP address with a small number of devices, they decide it is probably a household and assign all those devices to the same advertising profile. So, by being on the same wifi together (either at your place or hers) they will show ads on her devices based on your behavior (and vice versa).

* My guess would be: 1) Facebook (ie instagram) knows you are in a relationship. 2) Facebook knows girlfriend's location from being signed in (on Instagram). 3) Facebook knows locations are at open houses from data gathered from other users or around the web. Or maybe Facebook knows that going to a few totally new random residential locations in a short period of time, combined with girlfriend's other engagement activities means user is looking for a new place to live.

* The Facebook app tracks location and other peoples' locations, and makes assumptions based on people being at the same place at the same time. If Facebook (or whoever) knows that several other people are all interested in new houses, and all those people + your girlfriend go to the same place(s), Facebook decides that your girlfriend might have the same interest as all those other people.

* Android by default tracks your location constantly. I recently got a Pixel and was staying in a hotel. Every night I came back to the hotel room it would ask me to rate it or upload pictures of it to Google Maps. It can be disabled in Settings, iirc.

* Advertisers are really good at using available data to predict information that was never provided. In the case of the kung fu movie, it's possible IP address was used. For the open house, there could be some location correlation, but I would bet it's more than that (age, financial profile, relationship status). You can feed a bunch of data about someone to an algorithm and predict these things with pretty high confidence. The way to avoid this is to opt out of interest based ads. iOS and Android both have options for this.

Questions:

* Did you guys use an app (e.g. Zillow, Trulia) to look up listings?

* Did you invite her to come see the open house by texting her "hey, want to come see an open house"?

* Did she discuss looking at houses with you or anybody in emails or social media messages?

* Did her smartphone location ever correspond with a house that is listed on the MLS in the past week?

* Did either one of you login to amazon, Facebook, google, etc on one of the other persons device? If so there is likely still a tracking cookie associating you with her device, and your searches are causing her device to be targeted.
