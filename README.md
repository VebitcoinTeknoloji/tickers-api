# Vebitcoin Tickers API documentation

Vebitcoin coin instant Api document

## Usage For Single Cryptocurrency

You can add and use the api address you want to use in the system main url address.

System main url address: https://www.vebitcoin.com

Sample Api: /Ticker/Btc

Example usage: https://www.vebitcoin.com/Ticker/BTC

This sample will return Vebitcoin live market BTC (Bitcoin) tickers for last 24 hours.

## Usage For All Cryptocurrencies

Api: /Ticker/All

Example usage: https://www.vebitcoin.com/Ticker/All

This sample return Vebitcoin live market all coin tickers for last 24 hours.

## Request Limits

* .../Ticker/... requests are limited to 10 requests per 100 miliseconds.
* Other requests are limited to 1 request per 100 miliseconds.
* If you make more than 60 consequent unauthorized requests your IP address will be blocked.


## Ticker BTC (Bitcoin)

<code>GET</code> .../Ticker/Btc

**Result:**

```json
{
  "Code": "BTC"
  "Last": 37716.84,
  "High": 38303.14,
  "Low": 35659.84,
  "Vwap": 37037.64,
  "Volume": 32.6852999,
  "Bid": 37648.45,
  "Ask": 37716.84,
  "Time": "2017-11-26T13:29:26.21",
  "Open": 37268.57
}
```
* Last: Last BTC price.
* High: Last 24 hours price high.
* Low: Last 24 hours price low.
* Vwap: Last 24 hours volume weighted average price.
* Volume: Last 24 hours volume.
* Bid: Highest buy order.
* Ask: Lowest sell order.
* Time: Unix UTC timestamp date and time.
* Open : First price of the day.

## Available Tickers
*	BTC
*	LTC
*	ETH
*	XRP
*	ADA
*	XEM
*	TRX
*	QTUM
*	BCH
*	NEO
*	XLM
*	MIOTA
*	EOS
*	DASH
*	XMR
*	LSK
*	ICX
*	VEN
*	ETC
*	BTG
*	PPT
*	XRB
*	OMG
*	STEEM
*	ZEC
*	STRAT
*	SC
*	BCN
*	BTS
*	XVG
*	ZRX
*	SNT
*	WTC
*	MKR
*	ARDR
*	REP
*	WAVES
*	VERI
*	RHOC
*	DCR
*	AE
*	KMD
*	HSR
*	GAS
*	DRGN
*	KNC
*	ARK
*	LRC
*	BAT
*	DGB
*	ETN
*	ELF
*	DGD
*	PIVX
*	QASH
*	NAS
*	GBYTE
*	IGNIS
*	BTM
*	GNT
*	ZCL
*	IOST
*	CNX
*	R
*	FUN
*	ETHOS
*	AION
*	CND
*	PLR
*	FCT
*	DENT
*	SMART
*	SALT
*	POWR
*	GXS
*	NXT
*	MONA
*	XZC
*	NXS
*	SYS
*	MAID
*	RDD
*	ENG
*	REQ
*	SRN
*	PAY
*	BTX
*	ICN
*	WAX
*	PART
*	MED
*	GNO
*	LINK
*	GAME
*	QSP
*	EMC
