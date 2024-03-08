# Binance documentation

Binance USDs-M Futures API
Binance official supported Postman collections.


API documents: https://binance-docs.github.io/apidocs/futures/en/﻿

Telegram: https://t.me/binance_api_english﻿

Open Issue at: https://github.com/binance-exchange/binance-api-postman﻿

﻿

Market
﻿

GET
Test Connectivity
https://testnet.binancefuture.com/fapi/v1/ping
Test connectivity to the Rest API.

﻿

GET
Check Server Time
https://testnet.binancefuture.com/fapi/v1/time
﻿

GET
Exchange Information
https://testnet.binancefuture.com/fapi/v1/exchangeInfo
﻿

GET
Order Book
https://testnet.binancefuture.com/fapi/v1/depth?symbol=BTCUSDT
﻿

Query Params
symbol
BTCUSDT
limit
100
Default 100; max 1000. Valid limits:[5, 10, 20, 50, 100, 500, 1000]

GET
Recent Trades List
https://testnet.binancefuture.com/fapi/v1/trades?symbol=ETHUSDT
﻿

Query Params
symbol
ETHUSDT
limit
500
Default 500; max 1000.

GET
Old Trades Lookup (MARKET_DATA)
https://testnet.binancefuture.com/fapi/v1/historicalTrades?symbol=BTCUSDT
This endpoint need your API key only, not the secret key.

﻿

Query Params
symbol
BTCUSDT
limit
100
Default 500; max 1000.

fromId
''
GET
Compressed/Aggregate Trades List
https://testnet.binancefuture.com/fapi/v1/aggTrades?symbol=BTCUSDT
﻿

Query Params
symbol
BTCUSDT
fromId
startTime
endTime
limit
500
Default 500; max 1000.

GET
Kline/Candlestick Data
https://testnet.binancefuture.com/fapi/v1/klines?symbol=BTCUSDT&interval=1h
Kline/candlestick bars for a symbol. Klines are uniquely identified by their open time.

﻿

Query Params
symbol
BTCUSDT
interval
1h
1m, 1h, 1d

startTime
endTime
limit
500
Default 500; max 1500.

GET
Continuous Contract Kline/Candlestick Data
https://testnet.binancefuture.com/fapi/v1/continuousKlines?pair=&contractType=&interval=
Kline/candlestick bars for a symbol. Klines are uniquely identified by their open time.

﻿

Query Params
pair
contractType
interval
startTime
endTime
limit
GET
Index Price Kline/Candlestick Data
https://testnet.binancefuture.com/fapi/v1/indexPriceKlines?pair=BTCUSDT&interval=1h
Kline/candlestick bars for the index price of a pair. Klines are uniquely identified by their open time.

﻿

Query Params
pair
BTCUSDT
interval
1h
1m, 1h, 1d

startTime
endTime
limit
500
Default 500; max 1500.

GET
Mark Price Kline/Candlestick Data
https://testnet.binancefuture.com/fapi/v1/markPriceKlines?symbol=BTCUSDT&interval=1h
Kline/candlestick bars for the mark price of a symbol. Klines are uniquely identified by their open time.

﻿

Query Params
symbol
BTCUSDT
interval
1h
1m, 1h, 1d

startTime
endTime
limit
500
Default 500; max 1500.

GET
Mark Price