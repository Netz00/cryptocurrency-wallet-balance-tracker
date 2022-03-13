# Google sheets fetch and store "cron" job example

This script can be used for any other blockchain, just configure data fetching details(specific for that blockchain) \
and use it as that Blockchain wallet tracker.

Also it can be used for other Fetch and Store repeating operations, e.g. fetching Binance market trading pairs, \
or even in combination as fetching blockchain data and market data and doing some type of analysy.

## Blockchain Wallet Balanace Tracker

Simple way to track your wallet balance by using Google Sheets - Web app functionality.

[Live Preview](https://docs.google.com/spreadsheets/d/1-CHWN_lpJlKQTKm3HGBRV4gitopFQx2H1InrW8sTSLo/edit?usp=sharing)

INSTRUCTIONS

1. Go to google drive
2. Make new google sheet (new -> google sheets)
3. Add as many sheets as wallets you want to track + 1 sheet for Logfile
4. Call them e.g. "Idena1", "Idena2", ..., and "Log"
5. Go to Share -> Get link
    - e.g. https://docs.google.com/spreadsheets/d/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX/edit?usp=sharing
    - save somewhere "XX...XX" from link
6. Go to Extensions -> Apps Scripts
7. Overwrite default *Code.gs* with *Code.gs* from repository and change constants
8. Go to Deploy -> New Deployment -> Select type = Web App
    - Add Configuration
        - Any description
        - Execute As: Me
        - Who has access: Only myself
9. Press deploy
10. Set function initTriggers at Select function to run and press Run
11. Let it runs for few days, after that you will have enought great sample to calculate stats you are interested in.
    - Columns: { Timestamp, Balance, Stake, Sum } belong to script and any data added to that rows could be overwritten
    - For adding more stats just add functions to the free columns, starting from column "E"

---

This trivial example shows a brief look at huge abilities provided by google sheets.
 
Donation address: 0xD04483D8d9Aa7e83A4C12A30b89be353F30C440E
