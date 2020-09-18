---
layout: single
title:  "Boston Parking Tickets Data"
date:   2020-09-17 10:30:00 -0400
author: nstory
---
We recently received a response to our public records request to the City of Boston's [Transportation Department](https://www.boston.gov/departments/transportation), and it's a pretty cool set of records: [Boston parking tickets from 2018 to Aug 19, 2020](https://www.wokewindows.org/data_sources/parking_tickets). There are 3,200,977 tickets in this dataset!

At the <a href="https://www.wokewindows.org">Woke Windows Project</a>, our focus is on the Boston Police Department. While some parking tickets are written by Boston Police, most are issued by Parking Enforcement Officers, civilian employees of the Boston Transportation Department. So, consider this inaugural blog post a small diversion from what will be our usual programming.

Let's dig in and do some quick analysis of this dataset.

## Number of Tickets Issued

Let's sum the number of tickets issued in each month from January 2018 through July 2020 (I'm excluding August 2020 because that month is incomplete in our data).

![Tickets Issued by Month](/assets/images/parking_tickets/tickets_issued_by_month.png)
There is a definite seasonal trend with December through February being the slowest months for parking tickets.

![Tickets Issued by Month](/assets/images/parking_tickets/tickets_year_over_year.png)
Check out that decline starting in March 2020! COVID-19 had a dramatic impact on the number of tickets written.
This year-over-year chart shows us there was a 73% decline in tickets issued in April 2020 vs April 2019.

## Fine Amount
Let's look at the "Fine Amount" field.

![Tickets by Fine Amount](/assets/images/parking_tickets/tickets_by_fine.png)
The most common fines are between $25 and $49, accounting for 64% of all tickets written. The single most common amount is $40 which accounts for 51% of all tickets written.

![Fines by Month](/assets/images/parking_tickets/fines_by_month.png)
The highest total monthly levy was in October 2019 when $6.9MM in parking tickets were issued by the City of Boston.  Note that these numbers don't show how much the city actually took in from parking tickets, just the amount that was written on the tickets. This dataset doesn't take into account appeals, late penalties, and non-payment.

## Tickets by Vehicle Make
The parking ticket dataset has a field for the make (e.g. Ford, Toyota) of each car ticketed. Let's compare that to another dataset, the [Massachusetts Vehicle Census](https://www.mapc.org/learn/data/).

According to the Vehicle Census, there were 304,633 vehicles garaged in Boston in Q4 2014 (the most recent timespan available in that dataset). In 2018, there were 1,390,896 parking tickets issued in the City of Boston. That is *4.6 tickets per vehicle*.

Let's take the number of tickets each make received, and divide that by the number garaged in Boston:

![Tickets per Vehicle Make](/assets/images/parking_tickets/tickets_per_vehicle_make.png)
Manufacturers of commercial vehicles top this list. Vehicles made by Freightliner, which manufactures big-rig trucks, receive 41 tickets per vehicle garaged in Boston; that's 9x the average for all vehicles.

At the bottom of the list: Pontiacs receive 2 tickets per vehicle, Saturns receive 1.7 per vehicle, and, finally the least ticketed make is Mercury, with 1.6 tickets per vehicle.

## What's Next?
Are you looking for a cool project? Here are some ideas for what you can do with this dataset! If you implement anything, reach out to me, and I'll link to your work.

1. Map these records. Each ticket is labeled with a street address or intersection; <a href="https://en.wikipedia.org/wiki/Geocoding">geocode</a> this information to find the lat & long.
2. Break down tickets by the type of violation. Are certain types of violation found more often in particular neighborhoods?
3. Identify hot spots where tickets are often issued. Could confusing signage be to blame? See [Using FOIA Data and Unix to halve major source of parking tickets](https://mchap.io/using-foia-data-and-unix-to-halve-major-source-of-parking-tickets.html) for Matt Chapman's article detailing how he identified and fixed just such a problem spot using Chicago's parking ticket data.
4. Look at the tickets issued to commercial vehicles (where "Plate Type" = "CO").
5. Look at tickets starting with "AVR". These are "Abandoned Vehicle Reports".

Download the data here: [Boston parking tickets from 2018 to Aug 19, 2020](https://www.wokewindows.org/data_sources/parking_tickets)

## External Links
[Massachusetts Vehicle Census](https://www.mapc.org/learn/data/) the microdata spreadsheet has detailed information at the individual vehicle level

[City of Boston Parking Clerk](https://www.boston.gov/departments/parking-clerk) useful background information regarding parking tickets in Boston. See [Parking Ticket Fines and Codes](https://www.boston.gov/departments/parking-clerk/parking-ticket-fines-and-codes).

[See where Boston hands out the most parking tickets](https://www.bizjournals.com/boston/news/2017/09/27/see-where-boston-hands-out-the-most-parking.html) 2017 article from [Boston Business Journal](https://www.bizjournals.com/boston/) looking at parking ticket data

[Boston drivers’ choice: Parking tickets, the electric bill, lunch or diapers?](https://www.bostonherald.com/2019/06/02/boston-drivers-choice-parking-tickets-the-electric-bill-lunch-or-diapers/) 2019 article from the [Boston Herald](https://www.bostonherald.com/) on the financial impact parking ticket fines have on individuals

[The man who gives out the most parking tickets in Boston](https://www.bostonglobe.com/metro/2015/10/02/meet-man-who-gives-out-more-parking-tickets-boston-than-anyone-else/lf1BC6ocyTLccBMaMfsSCP/story.html) 2015 [Boston Globe](https://www.bostonglobe.com/) article
