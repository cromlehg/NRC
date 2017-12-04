<p align="center">
  <h1> GEN Shares Token</h1>
  <img src="./logo.png">
</p>


* _Standart_        : ERC20
* _Name_            : KIT - keep it transparent
* _Ticket_          : NRC
* _Decimals_        : 18
* _Emission_        : Mintable
* _Crowdsales_      : 2
* _Fiat dependency_ : No
* _Tokens locked_   : Locked

## Smart-contracts description

Contract mint bounty, advisors and founders tokens after each stage finished. 
Crowdsale contracts have special function to retrieve transferred in errors tokens.

### Contracts 
1. _NRCToken_ - 
2. _Presale_ - 
3. _ICO_ - 
4. _Deployer_ - 

### How to manage contract
To start working with contract you should follow next steps:
1. Compile it in Remix with enamble optimization flag and compiler 0.4.18
2. Deploy bytecode with MyEtherWallet. Gas 5100000 (actually 5019453).
3. Call 'deploy' function on addres from (3). Gas 4000000 (actually 3979551). 

You can withdraw coins from presale at any time after softcap reached. You should call function _withdraw_ to do this. 
All coins from presale transferred to special eth wallet, which specified in presale configuration.

After each crowdsale stage contract manager must call finishMinting. 

If softcap not reached investors can retrieve coins by calling refund after presale finished.

### How to invest
To purchase tokens investor should send ETH (more than minimum 0.1 EHT) to corresponding crowdsale contract.
Recommended GAS: 200000, GAS PRICE - 21 Gwei.

### Wallets with ERC20 support
1. MyEtherWallet - https://www.myetherwallet.com/
2. Parity 
3. Mist/Ethereum wallet

EXODUS not support ERC20, but have way to export key into MyEtherWallet - http://support.exodus.io/article/128-how-do-i-receive-unsupported-erc20-tokens

Investor must not use other wallets, coinmarkets or stocks. Can lose money.

## Main network configuration

* _Bounty_                     : 5% of total tokens
* _Founders_                   : 15% of total tokens
* _Bounty tokens wallet_       : 
* _Founders tokens wallet_     : 

### Crowdsale stages

#### Presale
* _Price_                      : 600 NRC per ETH
* _Minimal insvested limit_    : 0.01 ETH
* _Softcap_                    : 20 ETH
* _Hardcap_                    : 250 ETH
* _Start_                      : Wed, 20 Dec 2017 13:00:00 GMT
* _End_                        : Thu, 25 Jan 2018 13:00:00 GMT
* _Contract manager_           : 
* _ETH Wallets_                : , 0xEA15Adb66DC92a4BbCcC8Bf32fd25E2e86a2A770

_Milesto_

1. 1 week                      : +50%
2. 1 week                      : +40%
3. 2 week                      : +35%

#### ICO
* _Price_                      : 300 NRC per ETH
* _Minimal insvested limit_    : 0.01 ETH
* _Hardcap_                    : 1000 ETH
* _Start_                      : 25.12.2017 01:00 GMT
* _End_                        : 31.01.2018 00:00 GMT
* _Contract manager_           : 
* _ETH Wallets_                : 

_Milestones_
1. 1 week                      : +25%
2. 1 week                      : +10%
3. 2 week                      : +0%


