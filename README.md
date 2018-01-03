# arbitrage-moments
Finding the best arbitrage opportunities for the top 100 cryptocurrencies in python3.


`start [--pairs -p] [--exchanges -e] [--minimum_volume -m] [--simple -s] [--coins_shown -c]`

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

I usually run it with these settings:   
`start --exchanges Binance Kucoin Etherdelta Cryptopia Bittrex Bitfinex Poloniex --pairs ETH BTC LTC`

if you made some money, tips are appreciated and help further development.

coin|address
|---|---|
|LTC |`LPCyB2yExbZdJUNRyNhhV8EYD7zU5MqrX7`|
|BTC |`1GNUsALbvyNwYVGSsX7LGRKFtgdnH6s3Rg`|
|ETH |`0x293a25bc3e1da86bb3322cf940e7baf49f52cae4`|
