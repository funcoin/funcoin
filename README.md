Funcoin is just a clone of SmallChange which is a clone of Litecoin. This coin is created for fun and to learn and experiment. Do not use this for anything serious! :-)

If you want to build the wallet on Ubuntu, do the following:

- install dependencies

--sudo apt-get update
--sudo apt-get install build-essential libboost-all-dev libcurl4-openssl-dev libdb5.3-dev libdb5.3++-dev git qt-sdk libminiupnpc-dev libssl-dev

- clone this repo

git clone https://github.com/funcoin/funcoin.git

- build the wallet

qmake "USE_UPNP=-"
make

- add seed nodes (were not included in the source code)

in your home folder in .Funcoin, create Funcoin.conf and add the following:

addnode=95.85.15.176
addnode=95.85.8.14

*Note*: not guaranteed the nodes will be there :-)