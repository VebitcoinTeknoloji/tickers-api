# Vebitcoin Tickers API documentation

Vebitcoin coin instant Api document

Service has been moved to Google Cloud. Please use new  RESTFul API address

https://us-central1-vebitcoin-market.cloudfunctions.net/app/api

## Methods

### Pair Market Information

/ticker?sourcecoin=sourceCoinCode&targetcoin=targetCoinCode

Sample For : BTC/TRY market information.

ticker?sourcecoin=btc&targetcoin=try

Example usage: https://us-central1-vebitcoin-market.cloudfunctions.net/app/api/ticker?sourcecoin=btc&targetcoin=try
Return JSON

[
   {
      "Ask":42413.31,
      "Bid":42423.31,
      "High":42323.21,
      "Low":42267.04,
      "Price":42267.04,
      "Open":0,
      "Volume":171065.1603487092,
      "Time":"2018-09-23T09:04:32.760455Z",
      "SourceCoinCode":"BTC",
      "TargetCoinCode":"TRY"
   }
]

This sample will return Vebitcoin live market BTC (Bitcoin) / TRY (Turkish Lira) tickers for last 24 hours.

## All Market Information

/ticker

Return all markets information by pair.

Example usage: https://us-central1-vebitcoin-market.cloudfunctions.net/app/api/ticker

This sample will return all Vebitcoin live market pair all coin tickers for last 24 hours.

## Currency Prices

/ticker/coinCode

Vebitcoin has alternative ways to exchange. Forexample; user can exchange BTC with TRY and BTC with TUSD, or User can exchange XRP with BTC and XRP with TRY.
If you want to fetch information about Currency prices forexample XRP prices.

/ticker/xrp
Example usage : https://us-central1-vebitcoin-market.cloudfunctions.net/app/api/ticker/xrp

## Order Book (New)

/orderbook?symbol={marketPair}&limit={limit}

Vebitcoin allows you to access the order information of any market. This method gives the "BID" and "ASK" values on the market.

Symbol   : Market pair (xrpbtc,xrptry)
Limit    :Record count (0<limit<100)

Example  
https://us-central1-vebitcoin-market.cloudfunctions.net/app/api/?symbol=xrptry&limit=5

