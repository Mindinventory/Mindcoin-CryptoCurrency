Mindcoin integration/staging tree
================================

http://www.mindinventory.com

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2017-2018 Mindcoin Developers

What is Mindcoin?
----------------

Mindcoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total coins

The rest is the same as Bitcoin.
 - 20 coins per block
 - 2018 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the Mindcoin client sofware, see http://www.mindinventory.com


Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Mindcoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/mindcoin-project/mindcoin/tags) are created
regularly to indicate new official, stable release versions of Mindcoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Please follow below steps to setup GUI wallet in your LINUX system:

		$sudo apt-get update
		$sudo apt-get install build-essential libtool autotools-dev autoconf pkg-config libssl-dev libboost-all-dev qttools5-dev-tools

		$sudo add-apt-repository ppa:bitcoin/bitcoin
		$sudo apt-get update
		$sudo apt-get install libdb4.8-dev libdb4.8++-dev

		NODE INSTALLATION
		------------------
		$sudo curl https://raw.githubusercontent.com/creationix/nvm/v0.16.1/install.sh | sh
		$source ~/.profile
		$nvm install 0.10.25
		$nvm use 0.10.25

		$git clone https://github.com/malvikiran/mindcoin.git
		$cd mindcoin/
		$qmake "USE_UPNP=-"
		$make
	
		You will get a message stating there is no configuration file.
		$sudo gedit ~/.mindcoin/mindcoin.conf

		rpcuser=youruser
		rpcpassword=yourpassword
		daemon=1
		server=1
		connect=192.168.1.21
		listen=1

		$sudo ./mindcoin-qt // live mode

		$sudo ./mindcoin-qt -testnet //for testmode




# LICENSE!

MindCoin is [MIT-licensed](https://github.com/Mindinventory/Mindcoin/blob/master/LICENSE.txt).
     
## Let us know!
We’d be really happy if you send us links to your projects where you use our component. Just send an email to sales@mindinventory.com And do let us know if you have any questions or suggestion regarding our work.
