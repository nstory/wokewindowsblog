---
layout: single
title:  "Boston Public Records Log"
date:   2021-01-14 12:00:00 -0400
author: nstory
---

**EDIT Apr 14, 2021**

[Shawn Breen](https://twitter.com/TTOJAF) made a request for the Boston PRR log on MuckRock [FOIA Request: FOIA logs for years 2016, 2017, 2018, 2019 and 2020](https://www.muckrock.com/foi/boston-3/foia-request-foia-logs-for-years-2016-2017-2018-2019-and-2020-103036/). The data he received has the _Public Record Desired_ field for all requests, which makes the data much more useful.

The records he received, however, did not have the _Req. Compl. Date_ or _Request Status_ fields.

I combined the records originally described in this post with these new records to create a combined spreadsheet which includes all fields for requests from 2017 to 2020:

* [boston_prr_2017_2020.csv](https://wokewindows-data.s3.amazonaws.com/boston_prr_2017_2020.csv)
* [boston_prr_2017_2020.xlsx](https://wokewindows-data.s3.amazonaws.com/boston_prr_2017_2020.xlsx)

See also [the GitHub project](https://github.com/nstory/boston_public_records).

**Original Post**

The City of Boston responded to my public records request (PRR) for an export of the public records requests in the [Boston Public Records Center](https://bostonma.govqa.us/WEBAPP/_rs) (yeah, it's a little meta). These records were provided to me on Dec 8, 2020.

The log was provided to me as two files. One contains requests to the Boston Police Department (BPD), and one contains requests to all other departments. The police file does not contain a description of the records requested.

These logs are useful for at least two reasons:

1. You can use this list to get ideas for PRRs to make. This is a great way to learn from the requests made by experienced journalists, lawyers, and activists.
2. You can request copies of the public records already gathered for another party. This is potentially an easy way to get a lot of documents quickly.

I have two outstanding requests to the City of Boston for previously requested records based on these logs: [boston-public-records-responses-non-police-9407](https://www.foiamachine.org/foi/boston-public-records-responses-non-police-9407/?sharing=TFRNUJV10BD4) and [boston-public-records-responses-police-9408](https://www.foiamachine.org/foi/boston-public-records-responses-police-9408/?sharing=6Z2RNBW9SGDY)

Do you have any questions, ideas, or have you done anything interesting with this data? Reach out to me on Twitter [@nathan_story](https://twitter.com/nathan_story).

# Downloads

## PDF Files
These are the PDF files I received from the Director of Public Records:
[Boston_Police_Department_Public_Records_Requests.pdf](https://wokewindows-data.s3.amazonaws.com/Boston_Police_Department_Public_Records_Requests.pdf)
[City_of_Boston_Public_Records_Requests_Redacted.pdf](https://wokewindows-data.s3.amazonaws.com/City_of_Boston_Public_Records_Requests_Redacted.pdf)

## CSV Files
These are the CSV files I generated from the PDF files. Note: the `city_of_boston_public_records_requests_redacted.csv` file is not complete; it is missing pages 16, 22, 32. These pages contained redactions that prevented automatic conversion from the PDF.
[boston_police_department_public_records_requests.csv](https://wokewindows-data.s3.amazonaws.com/boston_police_department_public_records_requests.csv)
[city_of_boston_public_records_requests_redacted.csv](https://wokewindows-data.s3.amazonaws.com/city_of_boston_public_records_requests_redacted.csv)

## XLSX Files
These are the Excel files I generated from the PDF files. Note: the `city_of_boston_public_records_requests_redacted.xlsx` file is not complete; it is missing pages 16, 22, 32.
[boston_police_department_public_records_requests.xlsx](https://wokewindows-data.s3.amazonaws.com/boston_police_department_public_records_requests.xlsx)
[city_of_boston_public_records_requests_redacted.xlsx](https://wokewindows-data.s3.amazonaws.com/city_of_boston_public_records_requests_redacted.xlsx)

## Request
The message history for the public records request:
[R000673-091820_Message_History.pdf](https://wokewindows-data.s3.amazonaws.com/R000673-091820_Message_History.pdf)

## Source Code
See [https://github.com/nstory/boston_public_records](https://github.com/nstory/boston_public_records)
