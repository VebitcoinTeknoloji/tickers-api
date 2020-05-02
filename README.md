# Vebitcoin Tickers API documentation

Vebitcoin coin instant Api document

Please use new  RESTFul API base address

https://prod-data-publisher.azurewebsites.net/api

## Methods

### Pair Market Information

/ticker?sourcecoin=sourceCoinCode&targetcoin=targetCoinCode

Sample For : BTC/TRY market information.

ticker?sourcecoin=btc&targetcoin=try

Example usage: https://prod-data-publisher.azurewebsites.net/api/ticker?sourcecoin=btc&targetcoin=try
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

Example usage: https://prod-data-publisher.azurewebsites.net/api/ticker

This sample will return all Vebitcoin live market pair all coin tickers for last 24 hours.


## Order Book (New)

You can access the order information of any market. This method gives the "BID" and "ASK" values on the market.

{api-url}/orderbook?symbol={marketPair}&limit={limit}

Example usage : https://prod-data-publisher.azurewebsites.net/api/orderbook?symbol=xrptry&limit=5

## Trade Info (New)

You can access the transactions related trade. 

{api-url}/trades?symbol={marketPair}&limit={limit}

Example usage : https://prod-data-publisher.azurewebsites.net/api/trades?symbol=xrptry&limit=5

