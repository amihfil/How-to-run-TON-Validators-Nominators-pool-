# How to run TON Validators/Nominators pool
This is a very detailed guide on how to run node on the TON blockchain. The overall process devided into the small steps which are easy to follow.
##
### I. Running TON Validator
#### 1. Rent a server

It could be any server with the necessary resources mentioned on the ton validator page (8CPU, 64 GB RAM, 1TB storage and 1Gb internet speed)

#### 2. Install mytonctrl

Use standard instruction provided here https://github.com/NM005/mytonctrl

#### 3. Activate validator wallet

If you want to use a wallet that is already exists you have to install this software 

https://github.com/NM005/mnemonic2key

and dont forget add tonweb extension 

npm install tonweb

Then you have to start a generation of keys like in article and after this you will get 2 files in mnemonic2key directory .addr and .pk 

Then you need to put these keys in directory /mytoncore/wallets. It could new wallet or you can rename two new files to the names of existed local wallet and replace it

if you replace - you dont need to activate it, if you put a new wallt - just activate it using command aw.

#
### II. Running TON Nominators pool
#### 1. Update mytonctrl
#### 2. Create a pool for nominators
#### 3. Activate node as a nominator pool
#
Using nominator pool instead of validator to participate in rounds is a safer way. Because when you import their wallet, or transferring the entire stake to validator wallet, There is a vulnerability in the form of a server (which node), and which can be hacked and get full access to the entire stake. Nominators, on the other hand, transfer funds to a special smart contract that guarantees that only the nominator who made the deposit has access to these funds.
