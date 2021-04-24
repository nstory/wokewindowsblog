---
layout: single
title:  "Boston Traffic Citations 2011 - 2020"
date:   2021-04-24 01:00:00 -0400
author: nstory
excerpt: Updated traffic ticket data now covering tickets issued by Boston Police from 2011 through 2020
header:
  overlay_image: /assets/images/boston_traffic_citations/citation.png
  overlay_filter: 0.8
---

I just finished pushing updated traffic citation data to the [Woke Windows](https://www.wokewindows.org/) database.

Previously, Woke Windows just had the [traffic tickets written in 2019](https://www.wokewindows.org/data_sources/2019_tickets). Now we have data spanning the years 2011 through 2020.

These records have fields indicating: the Boston Police officer who wrote the ticket, the location where the ticket was written, the race and sex of the driver, and much more.

## Caveat
There is a discrepancy between the [2019 dataset](https://www.wokewindows.org/data_sources/2019_tickets) and the new [2011 - 2020 dataset](https://www.wokewindows.org/data_sources/2011_2020_citations).

There are 119 citations that appear in the 2019 dataset but do not appear in the new data.

I haven't identified a pattern to explain why these citations disappeared. If you have a theory, or if you have more MassDOT traffic ticket data I could compare against, please reach out!

## Get the data
There are a few ways you can access this data:
* Do you want to quickly browse all the tickets without downloading anything? Try the [big table of traffic citations](https://www.wokewindows.org/citations) on Woke Windows.
* Do you want to browse tickets written by a particular officer? [Look up an individual officer](https://www.wokewindows.org/officers) on Woke Windows and view all the data we have on that officer, including traffic tickets written.
* Do you want to download a spreadsheet which you can filter in Excel (e.g. take all the tickets written by one-or-more officers and then do an analysis based on location, race, etc.)? [Download data formatted for Excel](https://github.com/nstory/boston_pd_citations); these spreadsheets have been joined with Boston PD roster data, making it easy to identify the officer who wrote each ticket.
* Do you need the raw data provided by MassDOT? See [2011 - 2020 Traffic Tickets](https://www.wokewindows.org/data_sources/2011_2020_citations).

## Conclusion
Finally, if you are a developer, the source code is available on GitHub at [nstory/boston_pd_citations](https://github.com/nstory/boston_pd_citations) and [nstory/wokewindows](https://github.com/nstory/wokewindows).

Thank you to Josh Raisler Cohn for making the public records request for this data and sharing the response with me.
