# get-eth-balance

The site Etherscan allows you retrieve information on accounts and transactions. There is an interface to the Reposten testnet as well. While doing some work on a project I was monitoring the page to view an account balance and ended up creating a script to do the monitoring programmatically.

See blog post at [http://blog.bradlucas.com/posts/2017-07-27-ethereum-get-eth-balance-script/](http://blog.bradlucas.com/posts/2017-07-27-ethereum-get-eth-balance-script/)

## Setup

### Create virtual enviroment

```
$ python3 -m venv env
$ source env/bin/activate
```


### Install required libraries

```
$ pip install -r requirements.txt
```

## Usage


Command line Arguments:

```
-t use Ropsten testnet otherwise default to mainnet chain
-a account
```

Environment variables:
Use these in liu of the command line arguments

```
GET_ETH_BALANCE_CHAIN=[testnet|mainnet]        - Default to mainnet if not set
GET_ETH_BALANCE_ACCOUNT=account
```

Command line arguments will take precedence

```
$ python get-eth-balance.py -t -a 0xd60e64afb753583941e1ab42f836ced0d23af2db
```
