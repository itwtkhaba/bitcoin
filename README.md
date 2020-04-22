# Twenty One Community

**Idea**: I think we could make blockchain where 21 coins will be distributed among 21 * 100000000 addresses generated from genesis block hash. Each address should have 0.00000001 coin.

At start we should have 2 100 000 000 addresses with 0.00000001 coin at each address

We have to change bitcoin source code. All coins must be found in first block.

Coins found in frist block must be sent to 2 100 000 000 addresses. 1 address should have only 0.00000001 coin.

Addresses must be generated like pseudorandom address from genesis block hash without private or public keys. We need hardcode this in source code. 

Mining only needed for including transactions to blocks. Does not imply block reward or comissions and transaction fee reward. 

Transaction fee is zero.

21 coins at all.

Everybody may pseudomine coins with brute force addresses with balances. It's the only way to pseudomine coins. I think brute force is an honest way to distribute coins among users. Every user has equal chanses. No matter how much power, coins, wealth user has. It's only luck. 

Project not seeking the way to resolve transaction problem. This project create really rare asset for value storage. 
We could change PoW to PoS or DPOS consensus. Without rewards or fees. Every wallet may be full node.

Brute forcing addresses is not a waste of time. It's a chance. 

I'm looking for people who will support my idea and help me in developing. Absolutely open source. Developers, crypto enthusiasts, anarhists, blockchain developers we all need this system let's do it together. 

*Sorry for my English. I can read very well, but my writing skills are awful, I know.*

GPG: pgp.mit.edu 40FF484A75D43B88

Contacts:
Email: itwtkhaba@protonmail.com
GitHub: https://github.com/itwtkhaba
Reddit: itwtkhaba

Communities:

https://bitcointalk.org/index.php?topic=5242564.0

https://forum.bits.media/index.php?/topic/166062-%D1%81%D0%BE%D0%BE%D0%B1%D1%89%D0%B5%D1%81%D1%82%D0%B2%D0%BE-%D0%B4%D0%B2%D0%B0%D0%B4%D1%86%D0%B0%D1%82%D0%B8-%D0%BE%D0%B4%D0%BD%D0%BE%D0%B3%D0%BE/



Bitcoin Core integration/staging tree
=====================================

https://bitcoincore.org

What is Bitcoin?
----------------

Bitcoin is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. Bitcoin uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Bitcoin Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately usable, binary version of
the Bitcoin Core software, see https://bitcoincore.org/en/download/, or read the
[original whitepaper](https://bitcoincore.org/bitcoin.pdf).

License
-------

Bitcoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of Bitcoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and macOS, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

Changes to translations as well as new translations can be submitted to
[Bitcoin Core's Transifex page](https://www.transifex.com/bitcoin/bitcoin/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.

Translators should also subscribe to the [mailing list](https://groups.google.com/forum/#!forum/bitcoin-translators).
