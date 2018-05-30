# arbitrage-chances
Finding the best arbitrage opportunities for the top 100 cryptocurrencies.

### Dependencies
 + Cython - `python3 -m pip install cython`
 + Pymarketcap - `python3 -m pip install pymarketcap`
 

### Settings
`start [--pairs -p] [--exchanges -e] [--minimum_volume -m] [--simple -s] [--coins_shown -c] [--top -t] [--coin_list -l]`

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
+ `coin_list = []`
  + If set, runs on a set of specified currencies instead of the top X currencies
+ `top = 100`
  + sets the number of top currencies to use. It gets buggy towards the bottom (500s), so be warned.

I usually run it with these settings:   

### Recommended settings
`python3 ./start --exchanges Binance Kucoin Etherdelta Cryptopia Bittrex Bitfinex Poloniex --pairs ETH BTC LTC`

If this library helped you at all, you can donate ETH to `0x293a25bc3e1da86bb3322cf940e7baf49f52cae4`.

### Warning
+ Arbitrage usually exists for a reason. Usually this is:
  + No wallet withdrawal / Deposit for a coin
  + High withdrawal fees or long wait time
  + Very low volume
+ This library does not take any of these factors 
