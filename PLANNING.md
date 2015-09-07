# Kids activities planning sheets

(use at your own risk)

## 1. Create planning sheet for a single weekly activity

This is a planning for a single activity, taking place once a week.

* Visit https://docs.google.com/spreadsheets/d/17hifZh1Hce_4VnrXTvIo33TxV1ufqv2s5ch8LvGBK2w/edit?usp=sharing
* File -> Make a copy...
* Give it a title, save where you want
* Edit only the cells with red borders
  - day of week
  - starting from
  - names in "Total" box
  - names and comments in the planning
* Follow the instructions to enable automatic background colouring for cells with names
* Share -> "anyone with the link can view"
* Don't change anything else - or do so at your own risk

## 2. Create summary sheet for multiple weekly activities 

This is a summary page, grouping together multiple activities (pulled from separate spreadsheets) and displaying schedules for the coming weeks (for the nearest activity days).

* Visit https://docs.google.com/spreadsheets/d/1pKrAYgClUvH3F2FGPDJH4mCBBaY544wWs58QbMxFS-w/edit?usp=sharing
* File -> Make a copy...
* Give it a title, save where you want
* Fill in only the following columns - one row per activity
  - column A (activity name) - free text
  - column E (spreadsheet key = the long random text from the weekly planning spreadsheet URL)
* Delete unused rows
* Don't change anything else - or do so at your own risk
  - advanced: to import two cells into one, use something like `=CONCATENATE(IMPORTRANGE($E4, " !C1"), "/", IMPORTRANGE($E4, " !D1"))` 

## 3. Embedd the summary sheet on your personal "commuter info" page

Publish the summary sheet page:
* File -> Publish to the web...
* Embed
* not "Entire document", but "summary"
* Publish
* Copy the URL

Construct the URL your personal "commuter info" page:
* The general template for embedding an iframe with `URL` is `http://cern.ch/test-commuters-info/index.html#URL`
* For embedding Google Spreadsheets, use something like `http://cern.ch/test-commuters-info/index.html#https://docs.google.com/spreadsheets/d/XXXXXXXXXXXXXXXX/pubhtml?gid=YYYYYYYYYYY&single=true&chrome=false`
* Or best, use `http://test-commuters-info.web.cern.ch/test-commuters-info/index.html#` + the copied URL, without "widget" or "headers" arguments, but with `&single=true&chrome=false` at the end

