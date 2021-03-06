BitllCoin integration/staging tree
================================

http://www.bitllcoin.co

Copyright (c) 2009-2014 Bitcoin Developers

Copyright (c) 2017-2018 BitllCoin Developers

What is BitllCoin?
----------------

BitllCoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.

Algorithm -	Scrypt

Type - PoW

Coin name -	BitllCoin

Coin abbreviation - BTLLC

Address letter - L

RPC port - 30016

P2P port - 30015

Block reward - 100 coins

Block halving -	450000 blocks

Total coin supply -	100000000 coins

Premine percent - 10%

Premine amount - 10000000 coins


Coinbase maturity -	5 blocks

Target spacing - 2 minutes

Target timespan - 4 minutes

Transaction confirmations -	5 blocks


For more information, as well as an immediately useable, binary version of
the BitllCoin client sofware, see http://www.bitllcoin.co.

License
-------

BitllCoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the BitllCoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitllcoin-project/bitllcoin/tags) are created
regularly to indicate new official, stable release versions of BitllCoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./bitllcoin-qt_test

