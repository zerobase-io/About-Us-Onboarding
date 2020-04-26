![Zerobase Logo](./imgs/ZerobaseLogo.png "Zerobase Logo")

# Zerobase
Welcome! Zerobase is a free, privacy-first contact tracing platform that empowers individuals and local officials to stop the spread of COVID-19.

[Join us](https://zerobase.io/volunteer) in our fight to end COVID-19.

# About Zerobase
All things relating to our organization, the Zerobase project and how you can get involved!

## Contact Tracing
Contact tracing is the identification of likely disease-spreading interaction between individuals. It is a crucial part of modern pandemic response. If an individual is exposed to COVID-19, tracing allows us to identify any number of others who were in the same place, such as a grocery store, pharmacy, place of worship, or doctor’s office, at the same time as the infected person. Public health officials can then notify those people to stay home temporarily and/or get tested themselves, thus slowing the spread of the virus.

To contain COVID-19, communities must engage in both effective testing and tracing. While tests are scarce, we can respond by using contact tracing as soon as possible. Zerobase maximizes the value of each test by leveraging that test not only to treat an individual, but to identify the hundreds of untested members of a community who are at risk of infection based on their proximity to an exposed individual.

## How Does Zerobase Work?

Zerobase is a simple and effective tracing solution that can be used anywhere. Here’s how it works:

1. Paper printouts with unique Zerobase QR codes are posted at the entrances and touchpoints of public locations like grocery store cash registers, restaurant entrances, pharmacies, and banks.

2. People entering a participating location scan the code  – this is as simple as pointing a phone’s camera at the sign; it takes just a few seconds, and no app download is required. Here is an example code that you can scan right now:  

<p align="center">
    <img src="./imgs/sample_zerobase_qr.jpg" width="250" height="250">
</p>  

   Individuals may choose to share their phone number in order to be notified by public health authorities (or automatically by Zerobase, if so desired) if they have been exposed. By default, no personal information is collected.  

3. If an individual receives a COVID-19 test, they are given a sheet of paper or a sticker with a Zerobase QR code on it to scan as part of the intake process. Each code is unique and anonymous. Batches of code sheets can be printed at testing centers or distributed to drive-through sites. Then, a medical practitioner can scan the same code when a test result comes in to link the individual's anonymous trace with the test.

4. Zerobase anonymously analyzes community networks of interaction to identify people who visited the same places at roughly the same times. It then links an individual who has been tested to the individuals that they were near to construct a list of individuals that may have been exposed.

5. Public health officials can identify the community touchpoints through which the virus seems to be spreading most rapidly. They can also notify the individuals who may have been exposed and advise them to self-quarantine, even before they exhibit symptoms.

To see more about our system, read our [nontechnical whitepaper](zerobase-bluf.pdf).

## Why Zerobase?
Many great projects are tackling the contact tracing problem. We consider the people working on these efforts our siblings-in-arms and applaud their effort. Zerobase was designed to fill several significant holes in the present virtual contact tracing landscape.

### We are the only solution that does not require that everyone install the same app
Excluding systems that invasively track individuals' phones via their mobile provider, virtually all apps that attempt to do contact tracing utilize bluetooth proximity sensing, NFC, GPS monitoring, or similar technologies. These systems, while theoretically promising, require that individuals download an application to their phone and keep it open in the background all the time, which we believe will be an unclearable hurdle to widespread adoption. The bottom-up approach of convincing (even forcing) people to all install the same application and keep it active all the time is an extremely tenuous proposition in heterogenous populations. Instead, we rely on the fact that nearly every mobile device has a native QR scanner, meaning that everyone can be enrolled automatically and instantly.

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

# Volunteering and Contributing
We're so happy to have you! Where governments are unable or unwilling to adequately test people for CoV-SARS-2, we're here to bridge the gap by enabling even resource-poor communities to utilize advanced tracing techniques to contain infections.

You know how every job you've applied to tells you that you'll make an immediate impact? We don't even need to tell you how your contributions will matter, the value proposition of spending even a few hours contributing to a platform that is saving lives now speaks for itself. An investment of a few hours of your time will be directly responsible for eliminating days or weeks of unnecessary human suffering. So let's get to it!

### Register and Join our Slack

First, fill out our [Volunteer Registration Form](https://airtable.com/shrLF5neOHKjsSkjD) if you haven't already, [Join the Zerobase Slack](https://join.slack.com/t/necsi-edu/shared_invite/zt-d86ge6g0-sgLKgyhRpFBJq2VrnJOdhg), and introduce yourself in [#zerobase-volunteers](https://necsi-edu.slack.com/archives/C010FSAKGPQ)

#### Here our our main channels to get you started:
* [#zerobase-general](https://necsi-edu.slack.com/archives/CV57RBU8H) - Our main channel
* [#zerobase-onboarding](https://necsi-edu.slack.com/archives/C012TDJ6PEC) - Onboarding information
* [#zerobase-volunteers](https://necsi-edu.slack.com/archives/C010FSAKGPQ) - Our main volunteers channel

## Get Involved
Zerobase exists across 13 time zones and development and we use a decentralized team of teams structure. The best way to bring your best is to introduce yourself, join a team, partner up - and self start! Let us know how you would like to contribute, and we will support you in creating an impact!

Read our [core values](https://docs.google.com/presentation/d/1yxBwUKQG7YsQSvSuSaVimaDOZuh-HupIbDe9i3-GV_w/edit)

Read our [Zerobase Product Roadmap](https://github.com/zerobase-io/smart-tracing/wiki/Product-Roadmap) for up to date information of our current and focus - find out our biggest priority today, and what's coming next. If you want to understand why we are building what we are building today, start here.

Join our All Hands Meeting on Zoom every Tuesday, Wednesday and Saturday at 3:00 PM EST. Find the link every day on [#zerobase-general](https://necsi-edu.slack.com/archives/CV57RBU8H). Check team guides below for team specific zoom sessions.

### Join a Team and contribute!

#### Backend and Database Team
DBAs, Sys admins, CI/CD pros, NodeJS devs, Express experts, here's your home. Data scientists too!
* Team lead: David Harris
* Slack: [#zerobase-backend](https://necsi-edu.slack.com/archives/CV82ELK26)

#### CRM Team
Design, Create, Integrate, Automate, and Run the Customer Relationship Management system that runs our outreach, live deployments, and volunteer efforts.
* Team lead: Ed Kraay
* Slack: [#zerobase-crm](https://necsi-edu.slack.com/archives/C01219CJJHJ)
* [CRM Team Guide](https://github.com/zerobase-io/About-Us-Onboarding/blob/master/contributing/contributing-crm.md)

#### Design Team
* Slack: [#zerobase-design](https://necsi-edu.slack.com/archives/C010M0HCLSZ)

#### Deployments Team
Validated learning experts, user research gurus, iterative feedback afficionadoes. These people see to it that Zerobase is successful and improving on the ground. They also manage our support systems and ensure that problems get solved immediately.
* Team lead: Erik Sogn
* Slack: [#zerobase-deployments](https://necsi-edu.slack.com/archives/C010MA2D7PU)
* [Deployments Team Guide](https://github.com/zerobase-io/About-Us-Onboarding/blob/master/contributing/contributing-deployments.md)

#### Frontend Team - Design, UI/UX, and Medical
Web devs, mobile moguls, UI/UX experts, we especially need your help. We're so glad to have you!
* Team lead: John Lo
* Slack: [#zerobase-frontend](https://necsi-edu.slack.com/archives/C010DL0BXKR).

#### Infrastructure and Operational Security Team
DevOps, OpSec, K8s, and all the other fun shorthands - they live here!
* Team lead: Jason Spriggs
* Slack: [#zerobase-infra](https://necsi-edu.slack.com/archives/CV9UKU1HR).

#### Medical Team
We need experienced professionals in the healthcare and/or biomedical arena to help us bridge the gap between cloud technology and boots on the ground. Save lives by bringing about more effective rapid case identification and containment. Whether your expertise is running a gel or running an ICU, your knowledge is needed to help bring this system online quickly and to ensure best clinical utility.
* Team lead: Chris Lee
* Slack: [#zerobase-medical](https://necsi-edu.slack.com/archives/C011C9V9DQF)

#### Outreach Team
Grow zerobase by reaching and connecting us with invididuals, organizations, political leads, and movements that will forward our mission of saving lives by creating new opportunities for zerobase. If you have experience in law, communication, policy, social media, marketing, writing, or can recommend someone who does, we'd love to have your help in tackling this pandemic.
* Team lead: Bianca
* Slack: [#zerobase-outreach](https://necsi-edu.slack.com/archives/C011KJJH1NJ)
* [Outreach Team Guide](https://github.com/zerobase-io/About-Us-Onboarding/blob/master/contributing/contributing-outreach.md)

#### Product Team
Product and product managers, Jira jedi, and anyone else who considers organization to be a strong-point - your expertise is needed here.
* Team lead: Colm Byrne
* Slack: [#zerobase-product](https://necsi-edu.slack.com/archives/C0105T4K0F2)
* [Product Team Guide](https://github.com/zerobase-io/About-Us-Onboarding/blob/master/contributing/contributing-product.md)

#### Volunteer Coordination Team
Ensure volutneers join our project, get to the right place, and bring their best! Do you like to meet new people and set them up to win?
* Team lead: Erik Sogn
* Slack: [#zerobase-volunteer-coordination](https://necsi-edu.slack.com/archives/G0104HE1JP4)
* [Volunteer Coordination Team Guide](https://github.com/zerobase-io/About-Us-Onboarding/blob/master/contributing/contributing-volunteer-coordination.md)

#### Leadership Team
Are you passionate for organizational leadership theory and putting it into practice? Are you a technical founder or team builder? Are you committed to leading a team? Let us know. Want a high level view of what each team is focusing on? Check in here.
* Team lead: Aron Szanto
* Trello: [Leadership Trello](https://trello.com/b/7aDrFCR2/leadership)

# Any questions? Get stuck? Want to contribute and don't know where to start?
Email us at [info@zerobase.io](mailto://info@zerobase.io), ask in [#zerobase-volunteers](https://necsi-edu.slack.com/archives/C010FSAKGPQ), or use our [Contact Us](https://airtable.com/shrnYjRudkIBlXzr9) form.

# Links and Resources
* [Zerobase Volunteer Homepage](https://zerobase.io/volunteer)
* [Zerobase Product Roadmap](https://github.com/zerobase-io/smart-tracing/wiki/Product-Roadmap)
* [Zerobase GitHub Organization](https://github.com/zerobase-io)
