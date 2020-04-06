![Zerobase Logo](./imgs/ZerobaseLogo.png "Zerobase Logo")


# Zerobase
Welcome! Zerobase is a free, privacy-first contact tracing platform that empowers individuals and local officials to stop the spread of COVID-19.

[Join us](https://tinyurl.com/zerobase-volunteer) in our fight to end COVID-19.

# About Us & Onboarding
All things relating to our organization, the Zerobase project and how you can get involved!

## Contact Tracing
Contact tracing is the identification of likely disease-spreading interaction between individuals. It is a crucial part of modern pandemic response. If an individual is exposed to COVID-19, tracing allows us to identify any number of others who were in the same place, such as a grocery store, pharmacy, place of worship, or doctor’s office, at the same time as the infected person. Public health officials can then notify those people to stay home temporarily and/or get tested themselves, thus slowing the spread of the virus.

To contain COVID-19, communities must engage in both effective testing and tracing. While tests are scarce, we can respond by using contact tracing as soon as possible. Zerobase maximizes the value of each test by leveraging that test not only to treat an individual, but to identify the hundreds of untested members of a community who are at risk of infection based on their proximity to an exposed individual.


## How Does Zerobase Work?

We have developed a simple and effective tracing solution that is ready to be used in any community. Here’s how it works:

Zerobase is a simple and effective tracing solution that can be used anywhere. Here’s how it works:

1. Paper printouts with unique Zerobase QR codes are posted at the entrances and touchpoints of public locations like grocery store cash registers, restaurant entrances, pharmacies, and banks.

2. People entering a participating location scan the code  – this is as simple as pointing a phone’s camera at the sign; it takes just a few seconds, and no app download is required. Here is an example code that you can scan right now:  

<p align="center">
    <img src="./imgs/sample_zerobase_qr.jpg" width="250" height="250">
</p>  

   Individuals may choose to share their phone number in order to be notified by public health authorities (or automatically by Zerobase, if so desired) if they have been exposed. By default, no personal information is collected.  

3. If an individual receives a COVID-19 test, they are given a sheet of paper with a Zerobase QR code on it to scan as part of the intake process. Each code sheet is unique and anonymous. Batches of code sheets can be printed at testing centers or distributed to drive-through sites. Soon, we'll print these QR codes on stickers to place on the test kits themselves in order to match an anoymous trace network with a test result.

4. Zerobase anonymously analyzes community networks of interaction to identify people who visited the same places at roughly the same times. It then links an individual who has been tested to the individuals that they were near to construct a list of individuals that may have been exposed.

5. Public health officials can identify the community touchpoints through which the virus seems to be spreading most rapidly. They can also notify the individuals who may have been exposed and advise them to self-quarantine, even before they exhibit symptoms.

To see more about our system, read our [nontechnical whitepaper](zerobase-bluf.pdf).

## Why Zerobase?
Many great projects are tackling the contact tracing problem. We consider the people working on these efforts our siblings-in-arms and applaud their effort. However, Zerobase was designed to fill several significant holes in the virtual contact tracing landscape.

### We are the only solution that does not require that everyone install the same app
Virtually all other apps that attempt to do contact tracing utilize bluetooth proximity sensing, NFC, GPS monitoring, or similar technologies. These systems, while theoretically promising, require that individuals download an application to their phone and keep it open in the background all the time, which we believe will be an unclearable hurdle to widespread adoption. The bottom-up approach of convincing (even forcing) people to all install the same application and keep it active all the time is an extremely tenuous proposition in heterogenous populations. Instead, we rely on the fact that nearly every mobile device has a native QR scanner, meaning that everyone can be enrolled automatically and instantly.

### Other solutions do not account for how the virus actually spreads

Each existant modality of contact tracing suffers from at least one critical error. 

#### Bluetooth and NFC
Proximity sensing via bluetooth or NFC cannot account for indirect transmission, such as infection due to contact with a public touchpoints (a _fomite_, in the epidemiological jargon) like an ATM. Our system accounts for such transmission because we can link individuals through their mutual contact at a location that they were not at simultaneously. This defect also makes a peer to peer system blind to extremely important information about large clusters connected through a single fomite. Crucially, and in contrast with other applications we know of, our system is able to make strong claims about the risk associated with public locations with respect to the propensity of individuals to become infected due to their contact in that location. Both location and contact are first-class citizens, in contrast with bluetooth (contact) and GPS (location) models. We therefore provide a uniquely significant value proposition to public health officials who can act on this information in real time.

#### GPS location monitoring
GPS and cellular location data can be extremely imprecise, sometimes off by over 300 feet, especially indoors. Zerobase not only pinpoints the exact locations of community touchpoints, it is designed to focus on the specific high-traffic areas where the virus is most likely to spread - for example, inside buildings. And while platforms that track location data have history for their enrolled users, they are missing data for individuals who are not users of their platform. Zerobase is unique in that 100% of users are immediately enrolled via an instant check-in at all participating locations. GPS solutions also log locations for the 99.99% of the day that an infected individual spends not transmitting the virus. Instead, Zerobase homes in on the critical moments in public spaces that the infection may spread, making more accurate and focused determinations.

#### If you're tracking location, people have to know about and trust your solution to use it
Fundamentally, location tracking is both ineffective and unnecessary. Putting privacy first is critical to establishing trust and community buy-in. In many communities, there has been significant resistance to adopting more socially intrusive automated tracking and tracing methods. Community adoption and trustworthiness have been key design criteria since Zerobase’s inception. We believe in “Big Data without Big Brother.”

#### Collaborations
We fully expect that the eventual technical system that will be most effective for virtual contact tracing is a consortium solution, combining proximity, GPS, and touchpoint-based mechanisms (like ours). We have designed our system and models from the ground up to be able to quickly integrate with any other application that may provide helpful information. For example, we can easily ingest proximity events into our model by strengthening the affinity between nodes that were in the same place around the same time (per our touchpoint checkins) if we know that they were actually just a few meters apart via bluetooth. If you're working on another modality of contact tracing and want to team up to beat COVID-19, drop us a line at info@zerobase.io!

## How can I help?
Ready to jump in?

#### First, fill out our our volunteer form
[Zerobase Volunteer Registration Form](https://docs.google.com/forms/d/e/1FAIpQLSenbQaMHQTFyULEz7etYqM6X9sckrRwggbD5RMFqNpKT5AR4w/viewform)

#### Next, join our slack using this link
[Join the Zerobase Slack](https://join.slack.com/t/necsi-edu/shared_invite/zt-d86ge6g0-sgLKgyhRpFBJq2VrnJOdhg)

#### Join a team! These are some channels to get you started:
* [#zerobase-general](https://necsi-edu.slack.com/archives/CV57RBU8H) - Our main channel
* [#zerobase-backend](https://necsi-edu.slack.com/archives/CV82ELK26) - For backend developers
* [#zerobase-deployments](https://necsi-edu.slack.com/archives/C010MA2D7PU) - For deploying in the real world
* [#zerobase-frontend](https://necsi-edu.slack.com/archives/C010DL0BXKR) - For frontend developers, UX, and Medical
* [#zerobase-infra](https://necsi-edu.slack.com/archives/CV9UKU1HR) - For infrastructure and DevSecOps
* [#zerobase-product](https://necsi-edu.slack.com/archives/C0105T4K0F2) - Our main product channel

#### Check out our GitHub!
[Zerobase Developer Onboarding Documentation](https://github.com/zerobase-io/About-Us-Onboarding)
[Here's our quickstart guide for technical and nontechnical contributors. Join us!](./CONTRIBUTING.md)

#### Any questions? Get stuck?
Email us at [info@zerobase.io](mailto://info@zerobase.io) or ask in [#zerobase-volunteers](https://necsi-edu.slack.com/archives/C010FSAKGPQ)

Remember to join us at 4PM EDT for our daily worldwide All Hands call! Meet new friends, hear about our progress, become part of the team. Details on Slack.

#### Relevant Links
* [Zerobase GitHub Organization](https://github.com/zerobase-io)
* [Volunteer Registration Form](https://tinyurl.com/zerobase-volunteer)
* [Contact Us](https://airtable.com/shrnYjRudkIBlXzr9) or email us at info@zerobase.io
