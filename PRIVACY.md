# Privacy & User Data Management

## Table of Contents
* [What Data Does Zerobase Collect?](#what-data-does-zerobase-collect)
    * [User Data Collection Policies](#user-data-collection-policies)
    * [Business & Location Data Collection Policies](#business-location-data-collection-policies)
* [Are Your Data Policies The Same In All Countries?](#are-your-data-policies-the-same-in-all-countries)
* [How Is My Data Anonymized?](#how-is-my-data-anonymized)
* [How And Where Does Zerobase Store My Data?](#how-and-where-does-zerobase-store-my-data)
    * [Firebase Notification System](#firebase-notification-system)
    * [Mongo or Neo4J Tracing System](#mongo-or-neo4j-tracing-system)
* [What Data Is Available To Public Health Officials?](#what-data-is-available-to-public-health-officials)
* [What Extra Data Can I Voluntarily Provide?](#what-extra-data-can-i-voluntarily-provide)
    * [How Will You Use That Data?](#how-will-you-use-that-data)

## What Data Does Zerobase Collect?

#### User Data Collection Policies

#### Business & Location Data Collection Policies

## Are Your Data Policies The Same In All Countries?

## How Is My Data Anonymized?

## How And Where Does Zerobase Store My Data?
Be ready for some technical details!

#### Firebase Notification System
As part of our mobile app, we send out push notifications to users when we believe they were exposed to someone carrying CoV-SARS-2.
In order to do this, and to keep an accurate log of notifications we send, Zerobase utilizes Google's Firestore nonrelational database
to record when we broadcast a new potential exposure and to facilitate the sending of those messages.

The Firestore `/exposures` collection stores the device fingerprint for locations/businesses whose visitors need to be notified of a
potential exposure. **This device fingerprint never leaves Firestore**, as this collection cannot be queried outside of the internal
Firebase functions and the administrative console. **We will never expose this data directly.** It is theoretically possible for an
extremely motivated individual to be able to deduce which location's fingerprint was used to send these messages, but this attack would
be highly impractical and is completely unavoidable if we only notify people who visited a location when that location may have exposed
them. This fingerprint cannot be stored more securely while still fulfilling its purpose.

Additionally, a log of the locations that user has visited could be derived from the data stored by Firebase to administrate our
Firebase Cloud Messaging system, but this is not data we're storing ourselves, meaning that the security of this data has been vetted
very thoroughly by engineers at Google. **This data is never publicly exposed, and lives only within highly secure internal Firebase 
systems.**

#### Mongo or Neo4J Tracing System

// #### Others, as created

## What Data Is Available To Public Health Officials?

## What Extra Data Can I Voluntarily Provide?

#### How Will You Use That Data?
