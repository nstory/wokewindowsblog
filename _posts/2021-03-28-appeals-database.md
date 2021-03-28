---
layout: single
title:  "Public Records Appeals Database"
date:   2021-03-28 01:00:00 -0400
author: nstory
excerpt: Introducing a searchable database of Massachusetts public records appeals.
header:
  overlay_image: /assets/images/appeals_database/header.png
  overlay_filter: 0.9
---

I just pushed live a new feature on Woke Windows: a [searchable database of Massachusetts public records appeals](https://www.wokewindows.org/appeals).

Using this database, you can search appeals made to the Secretary of the Commonwealth, including the text of determinations issued by the Commonwealth's Supervisor of Records (while the Commonwealth does provide [a page for searching appeals](https://www.sec.state.ma.us/AppealsWeb/AppealsStatus.aspx), it does not allow for full text searches).

A requestor of public records will typically file an appeal when an agency or municipality does not respond to a request, denies access to a record, or is otherwise unreasonable. The Supervisor will then weigh in, and, if the agency is not complying with the law, issue an order for the agency to do so. See [A Guide to the Massachusetts Public Records Law](https://www.sec.state.ma.us/pre/prepdf/guide.pdf) for the full story.

## How is this useful?

The appeals are full of useful information that can inform your own public records requests.

*Are you curious what stories the Boston Globe is working on?* Search the database for [appeals containing "boston globe"](https://www.wokewindows.org/appeals?q=%22boston+globe%22).

*Are you interested in the files available from some agency, but don't know what to ask for?* Search the database for appeals relating to that agency (e.g. [The Board of Registration in Medicine](https://www.wokewindows.org/appeals?q=custodian+%7E%22board+of+registration+in+medicine%22)) and read the decisions; see what other requestors ask for.

## Can I use this to get records?
Yes!

As an example, I'll show you how I was able to use this database to get the Internal Affairs log for the [Everett Police Department](https://everettpolicema.com/).

First run a search for [everett police internal affairs](https://www.wokewindows.org/appeals?q=%22everett+police%22+%22internal+affairs%22):
!["everett police" "internal affairs" search results](/assets/images/appeals_database/search_results.png)

Of the cases returned, [Appeal #20201532](https://www.wokewindows.org/appeals/20201532) is particularly interesting. According to the determiniation [spr201532.pdf](https://wokewindows-data.s3.amazonaws.com/appeals/16957/spr201532.pdf), it regards a request for "all alleged misconduct complaints filed with the Everett Police Department during calendar years 2010 through 2019."
![copies of records that describe all alleged misconduct complaints filed with the Everett Police Department during calendar years 2010 through 2019](/assets/images/appeals_database/first_para.png)

The last paragraph of the determination orders "A copy of any such response must be provided to this office."
![A copy of any such response must be provided to this office](/assets/images/appeals_database/last_para.png)

This means it's likely the Supervisor of Records now has a copy of these files. So, I sent a public records request to the [Secretary of the Commonwealth's Records Access Officer](https://www.sec.state.ma.us/pre/prepra/prasecrao.htm):

![Public Records Request: Records provided for SPR20/1356 and SPR20/1532](/assets/images/appeals_database/nstory_prr.png)

Six days later I received a response:

![Please find attached responsive records](/assets/images/appeals_database/prr_response.png)
[Download the Everett SPR20/1356 and SPR20/1532 files](https://wokewindows-data.s3.amazonaws.com/everett_responses.zip)

Why is this exciting? For the original requester to get these files, he went through a two month process including two appeals. We were able to get the same files in a fraction of the time.

It won't always be the case that the Supervisor of Records will have an electronic copy of an agency's response. In those cases, you can either:
* reach out to the original requestor (while public records requests and appeals can be made anonymously, most people choose to include their name and organization; you can Google them)
* or make a request to the original agency and ask for any records they sent to the requestor

## Finally
Have any questions, comments, ideas? Reach out to me [@nathan_story](https://twitter.com/nathan_story) or by email nstory (at) wokewindows (dot) org.

## Links
* [Appeals — The Woke Windows Project](https://www.wokewindows.org/appeals)
* [nstory/wokewindows](https://github.com/nstory/wokewindows) &mdash; source code for the Woke Windows Project including the appeals database
* [nstory/public_records_division](https://github.com/nstory/public_records_division) &mdash; source code for scraper and links to data files for download
* [Appeals Tracking System: Search for an appeal](https://www.sec.state.ma.us/AppealsWeb/AppealsStatus.aspx) &mdash; the state's interface for searching appeals
