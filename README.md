# About Us & Onboarding
All things relating to our organization, the Zerobase project and how you can get involved!

## Table of Contents
* [What is Zerobase?](#what-is-zerobase)
* [How Do I Use Zerobase?](#how-do-i-use-zerobase)
* [How Can Zerobase Keep My Identity Secret AND Use My Data?](#how-can-zerobase-keep-my-identity-secret-and-use-my-data)
    * [How is Zerobase Implemented?](#how-is-zerobase-implemented)
* [How Can I Contribute to Zerobase?](#how-can-i-contribute-to-zerobase)
    * [Relevant Links](#relevant-links)

## What is Zerobase?
At its core Zerobase is a location tracker for community hot spots. Businesses, organizations, locations use a designated smartphone to enroll, print out a QR code and request that every individual entering the premise scan the code. We work with public health agencies to then backtrace potential exposure events in the case that an individual tests positive and notify all affected locations and individuals with next steps.

We offer unparalleled privacy for users by utilizing innovative and powerful cryptography, so you can trust that this extremely serious
data relating to an individual's CoV-SARS-2 exposures is infeasible to tamper with and kept highly anonymized. Additionally, we're 100% 
open-source, so anyone can audit our code for security and/or privacy concerns at any time. 

If you're looking for a further explanation of who we are and what we're doing, check out our [one-page mission statement and
organizational summary](./Zerobase-Basic.pdf).

## How Do I Use Zerobase?
// Brief overview of basic user flows

## How Can Zerobase Keep My Identity Secret AND Use My Data?
We cover this in great detail in [our privacy statement](./PRIVACY.md), including techinical and implementation details. But if you want
the short version, the answer is *public key cryptography*. Imagine you have two unique cans of paint, and you pour out a little bit of
each can into a cup and stir it until completely mixed. If I asked you to look at the two cans of paint and tell me if their combination
was the same color as the paint in our cup, it would be easy to answer, "yes, those two colors mix into this third one." But if asked to
determine the colors of the paint in the cans given *only* the color of the mixed paint in the cup, this is obviously an unfair problem!
There is no simple way to unmix two colors of paint, your only option would be to go to the store, buy a can of every single color of
paint and try every possible combination until you got lucky and figured it out via brute force. That would take a very long time! This
example illustrates what a "trapdoor" function is: it's easy to verify that some inputs result in a given output, but it's infeasible
to reverse this and figure out the inputs from only a given output. Using this powerful "easy-forwards, hard-backwards" principal and
some clever mathematics, we can have all users store some data that uniquely identifies them (their "private key") and use that as in 
input for a function whose output we store in our databases. This way, we can have the user prove their identity by asking them a 
question that requires their private key to answer, but we don't ever actually store that private key ourselves. We can then use their
data without exposing their identity AND maintain knowledge of who's who by storing the output of one of these special trapdoor 
functions.

#### How Is Zerobase Implemented?
If you're still curious and want to learn more, see [our privacy statement](./PRIVACY.md) for the specifics of how we provide this 
service with an unrivaled promise of privacy, or visit 
[the Wikipedia page for Public Key Cryptography](https://en.wikipedia.org/wiki/Public-key_cryptography) for the mathematics and further 
explanations of how such systems guarantee privacy and authenticity. Additionally, we're 100% open-source, so if you want to see how
something works or how your data is handled, you can view our source code directly. The only thing you *can't* see is our private user
data.

## How Can I Contribute to Zerobase?
Ready to jump in? [Here's where you can start!](./CONTRIBUTING.md)

#### Relevant Links
* Zerobase GitHub Organization: https://github.com/zerobase-io
* Zerobase Slack: https://necsi-edu.slack.com/archives/CV57RBU8H
* Volunteer Sign Up Sheet: https://docs.google.com/spreadsheets/d/1zCCdLi4jRecI9HlJYk3SqoQ-Md62TB2ub3Hgwgq6LYU/edit#gid=0
