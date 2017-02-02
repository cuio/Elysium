Elysium integration/staging tree
================================



What is Elysium?
----------------
Elysium is a P2P crypto-currency which is set to revolutionize the world by being the first Crypto-currency for Governments for Global Settlement Network and a Crypt-currency facilitating trade, commerce and investments worldwide through its disruptive technology .

 - 60 seconds block targets
 - Block halving in 1,20,000 Blocks
 - ~Total coin supply	18,000,000 ( 18 Million ) 
 - 60 coins per block
 - Algorithm :- Scrypt
 - Type	:- PoW
 

The word Elysium comes from ancient greek word Ἠλύσιον πεδίον , as a conception of the afterlife that developed over time , it expanded to include those chosen by the gods, the righteous, and the heroic, where they would remain after death, to live a blessed and happy life, and indulging in whatever employment they had enjoyed in life.

In Homer’s Odyssey, Elysium is described as a paradise:
to the Elysian plain…where life is easiest for men. No snow is there, nor heavy storm, nor ever rain, but ever does Ocean send up blasts of the shrill-blowing West Wind that they may give cooling to men.

License
-------

Elysium is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Elysium
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/elysium-project/elysium/tags) are created
regularly to indicate new official, stable release versions of Elysium.

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
    ./elysium-qt_test

