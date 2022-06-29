# PoliticianStock

## Overview

If politicians are able to trade with insider knowledge, why can't we? Politicians are required to provide details on their personal finances annually, however many will periodically submit these reports. PoliticianStock is an API that gathers U.S. House Representative and Senators stock trade information and provides developers with an easy way to access these transactions!

## Problem / Project Origins

Currently there are no ready-to-use APIs that have access to stock trades of all members of Congress. Most require web scraping or significant data transformation. This project aims to deliver an API that is easy to use, provides transformed data, and is publicly available.

## Completed

-   The Web Scraper to obtain stock information
-   Data Transformation for the custom object for the NoSQL DB
    -   The reason that I started with a NoSQL DB is because I was using google Firebase. It's really easy and quick to setup and I've had a lot more experience with these technologies.
    -   For an MVP/POC it was fine to start, but now that the project is getting more complex, it's time to think more about versatile querying of the data.

## Work In Progress

-   Designing the relational tables for more versatile API requests
-   Adding SQLAlchemy to the project to handle the relational db

### Moving from non-relation to relation DB

Currently, the data is in a NoSQL DB. This was due to the ease of starting the project and Google Firebase integration. Moving it to a SQL DB would be beneficial because we can create more versatile APIs.

In the NoSQL DB, the only optimized request is GET all transactions on a particular date. With how data is stored in a non-relational DB, we would have a lot of repeated data to have the same flexibility when creating APIs compared to a relational DB. An example could be getting all trades of a particular person in power. That would require restructuring of the data or having repeated content.

## Where To Find

I will update this with a link once the project is up and runnning. Stay tuned :)
