# arbitrage-chances
Finding the best arbitrage opportunities for the top 100 cryptocurrencies.

Dependencies:
 + Cython - `python3 -m pip install cython`
 + Pymarketcap - `python3 -m pip install pymarketcap`
 
`start [--pairs -p] [--exchanges -e] [--minimum_volume -m] [--simple -s] [--coins_shown -c] [--top -t]`

defaults:
+ `trading_pairs = ALL`
  + sets what trading pairs are accepted
+ `exchanges = ALL`
  + sets what exchanges are accepted
+ `minimum_volume = 1%`
  + sets minimum coin percent volume on exchange
+ `simple = False`
  + hides information and errors
+ `coins_shown = 10`
  + sets the number of coins shown
+ `top = 100`
  + sets the number of top currencies to use. It gets buggy towards the bottom (500s), so be warned.

I usually run it with these settings:   
`python3 ./start --exchanges Binance Kucoin Etherdelta Cryptopia Bittrex Bitfinex Poloniex --pairs ETH BTC LTC`

If you want a feature, please open an issue! Thanks.

coin|address
|---|---|
|LTC |`LPCyB2yExbZdJUNRyNhhV8EYD7zU5MqrX7`|
|BTC |`1GNUsALbvyNwYVGSsX7LGRKFtgdnH6s3Rg`|
|ETH |`0x293a25bc3e1da86bb3322cf940e7baf49f52cae4`|

Note:
+ Arbitrage usually exists for a reason. Usually this is:
  + No wallet withdrawal / Deposit for a coin
  + High withdrawal fees or long wait time
  + Very low volume
 
