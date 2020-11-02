

# Q&A about Nodl
  - [Disclaimer](#disclaimer)
  - [List of questions and definitions](#list-of-questions-and-definitions)
  - [Knowledge you should be confidently applying](#knowledge-you-should-be-confidently-applying)
  - [Actions you should be comfortable with](#actions-you-should-be-comfortable-with)
  - [Jump table to categories](#jump-table-to-categories)

Inspired by questions asked on the open [Nodl Telegram-group]https://web.telegram.org/#/im?p=@nodl_it), but also the open Telegram *Nodl Support* group [here](https://web.telegram.org/#/im?p=@nodl_support) and [Twitter @Nodl_it](https://twitter.com/nodl_it).

Beware: A Q&A is always *work in progress*. Tips & help welcome.

### Disclaimer
None of the respondents in the **open** Telegram groups nor Tweets have been explicitly named as a source, except for ***@Ketominer***, ***@Fonta1n3***. For practical reasons educational images uploaded by Github members, Telegram group members en Tweeps have been downloaded. We de-personalised them by giving images a new name. Under these new names these images have been uploaded to github and used in the Q&A to clarify the questions and answers.

We've done our best to protect the privacy of the Github, Telegram group members and Twitter accounts by investigating the images we used. We haven't come across personal identifiable information (pii). However, should we have made a mistake after all, please let us know and we'll correct this immediately.

### List of questions and definitions

- [Definitions](#definitions)<br/>
- [Q&A section General](#q-a-section-general)
  * [What is the Gordian System?](#what-is-the-gordian-system-)
  * [Why use the Gordian System?](#why-use-the-gordian-system-)
  * [What OSes can the Gordian System run on?](#what-oses-can-the-gordian-system-run-on-)
- [Q&A section Userinterface](#q-a-section-userinterface)
- [Q&A section Gordian Server](#q-a-section-gordian-server)
  * [Where can I download Gordian Server?](#where-can-i-download-gordian-server-)
  * [What kind of compromises would Gordian have to make in order to be distributed via the mac app store?](#what-kind-of-compromises-would-gordian-have-to-make-in-order-to-be-distributed-via-the-mac-app-store-)
  * [If I allready have a full node running on my Mac. Can I use the Gordian Server app with it?](#if-i-allready-have-a-full-node-running-on-my-mac-can-i-use-the-gordian-server-app-with-it-)
  * [I am about to start a full node on Mac. Can I change the directory to an External SSD with the Gordian Server StandUp App?](#i-am-about-to-start-a-full-node-on-mac-can-i-change-the-directory-to-an-external-ssd-with-the-gordian-server-standup-app-)
  * [Why does the `tor` service persist in the background even after I've shut down Gordian Server? Why doesn't Gordian Server shut down its service that it initiated?](#why-does-the--tor--service-persist-in-the-background-even-after-i-ve-shut-down-gordian-server--why-doesn-t-gordian-server-shut-down-its-service-that-it-initiated-)
        * [Further question: Most people would expect it to stop itself when pressing `cmd+q`? Most people think of apps in macOS as a self contained monolith.](#further-question--most-people-would-expect-it-to-stop-itself-when-pressing--cmd-q---most-people-think-of-apps-in-macos-as-a-self-contained-monolith)
        * [Further answer:](#further-answer-)
- [Q&A section Backup and Restore](#q-a-section-backup-and-restore)
  * [How does one restore QR vault if you've lost your iPhone?](#how-does-one-restore-qr-vault-if-you-ve-lost-your-iphone-)
- [Q&A section Gordian Wallet](#q-a-section-gordian-wallet)
  * [What’s the difference between Gordian Wallet (GW) and Fully Noded (FN)?](#what-s-the-difference-between-gordian-wallet--gw--and-fully-noded--fn--)
  * [There is no “add manually” like in FullyNoded?](#there-is-no--add-manually--like-in-fullynoded-)
- [Q&A section Fully Noded](#q-a-section-fully-noded)
- [Q&A section Connection](#q-a-section-connection)
- [Q&A section Node](#q-a-section-node)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## Knowledge you should be confidently applying
- The definitions above
- BIP32, BIP39, BIP44, BIP47, BIP49, BIP84, BIP174
- derivation paths, keypools
## Actions you should be comfortable with
- Amend knowledge and keep existing knowledge up to date
- recover from a seed
- sweep to a new wallet
- use bitcoin-cli
- install, sync, start and stop your own full node
- connect your TOR V3

# Jump table to categories
- [General](#q-a-section-general)
- [Userinterface](#q-a-section-userinterface)
- [Nodl administrator](#q-a-section-nodl-administrator)
- [Backup and Restore](#q-a-section-backup-and-restore)
- [Wallets](#q-a-section-wallets)
- [Connection](#q-a-section-connection)
- [Node](#q-a-section-node)

# Definitions
##### Apple id
: a login and password to keep your settings and Apple services up to date on all of your devices. Just sign in with the same Apple ID everywhere.
##### bech32  bitcoin address(p2wpkh)
:BIP49 refers to the accepted common standard of deriving segwit "compatibility" addresses. These addresses begin with a 3.
##### BIP84 keys 
: BIP84 refers to the accepted common standard of deriving native segwit addresses. These addresses always begin with bc1 - and are referred to bech32 addresses.
##### bitcoin.conf
: The bitcoin configuration file is a list of 'setting=value' pairs, one per line, with optional comments starting with the '#' character. 
##### Bitcoin-cli
: Bitcoin *CommandLine Interface*; just like Bitcoin Core app the CLI uses RPC calls to give your node and the bitcoin network commands and get results back.
##### Bitcoin Core (Wallet) App, also known as `Bitcoin-qt`
: Software running on MacOS, Windows and Linux that offers a **Graphical User Interface** to your Bitcoin Wallet and, if you wish, to your node. Just like Bitcoin CLI the Core app uses RPC calls to give your node and the bitcoin network commands and get results back.
##### Bitcoin-qt
: another name for Bitcoin Core (Wallet) App.
##### bitcoind
: Bitcoin Deamon, background process running a bitcoin node. Bitcoind is a program that implements the Bitcoin protocol for remote procedure call (RPC) use. It is also the second Bitcoin client in the network's history. It is available under the MIT license in 32-bit and 64-bit versions for Windows, GNU/Linux-based OSes, and Mac OS X. [Read more](https://en.bitcoin.it/wiki/Bitcoind)
##### bitcoind
: Bitcoin Deamon, background process running a bitcoin node. Bitcoind is a program that implements the Bitcoin protocol for remote procedure call (RPC) use. It is also the second Bitcoin client in the network's history. It is available under the MIT license in 32-bit and 64-bit versions for Windows, GNU/Linux-based OSes, and Mac OS X. [Read more](https://en.bitcoin.it/wiki/Bitcoind)
##### coldcard 
: a type of hardware wallet to store, send and receive crypto currencies
##### Datadir
: The data directory is the location where Bitcoin's data files are stored, including the wallet data file.
##### Esplora 
: Name of Blockstream's Tor V3 api to broadcast, it falls back to the users node if the api is unavailable. More info [here](https://github.com/Blockstream/esplora)
##### FN
: Fully Noded app
##### FN2
: see GW
##### Fully Noded wallets
: support BIP39 recovery words, the seed is encrypted and stored on your device **not** on the node. The node will only ever hold public keys. Your node will build psbt for us that FN will sign (not your Node). Your node verifies the UTXO's
##### GW 
: Gordian Wallet, formerly known as `Fully Noded 2` app, The original name FN2 was a misnaming because it is a different app than FN from its inception. [This comparison](http://github.com/henkvancann/FNcompGordian/FN2_Comparison.md) tries to explain the differences between Fully Noded and Gordian Wallet.
##### gap limit 
: This means you ended with more than 20 consecutive unused addresses in your bitcoin wallet. This could have have happened due to various reasons. [What it is and how to get over it](https://blog.blockonomics.co/bitcoin-what-is-this-gap-limit-4f098e52d7e1)
##### Initial block download (IBD)
: The Bitcoin Core initial block download code makes sure that the block headers you are downloading (from a single peer) passes certain, hard-coded "checkpoints.
##### Keepkey 
: a type of hardware wallet to store, send and receive crypto currencies
##### keypool 
: The keypool is a collection of unused addresses in your wallet. The keypool parameter tells the client how many unused addresses to keep in its pool. The original purpose of the keypool is to allow you to backup your wallet file less frequently and still have access to all your funds in the event of a hard drive failure. However since the invention of Hierarchical Deterministic Wallets (HD wallets, [BIP32](https://en.bitcoin.it/wiki/Deterministic_wallet)): If you have a HD wallet (check the icon on the bottom-right corner in Bitcoin Core), it doesn't matter. If you've created your wallet in an older version of Bitcoin Core, it's not an HD wallet. If that's the case, your keypool is important for backups: your backup has the same 1000 keys, which means you only need to make a new backup after using many different new addresses. If you would limit the keypool size to 20, you'll quickly run out of addresses, and you need to make new backups very often. That's the reason the keypool was increased from 100 to 1000. An important distinction with regrads to FN and Bitcoin Core is that Bitcoin Core is not able to add multisig addresses to the keypool, therefore we rely on the `bitcoin-cli` command `deriveaddresses` to derive multisig addresses on the fly using your multisig descriptors.
##### legacy bitcoin address (p2pkh)
: refers to the accepted common standard to derive non segwit addresses. These addresses always begin with a 1.
##### Libwally 
: an open source library (https://github.com/ElementsProject/libwally-core) used by Fully Noded, (https://github.com/blockchain/libwally-swift/blob/master/README.md) which allows us to utilize BIP39 directly in the app meaning you can easily recover your Fully Noded wallet with Electrum for example. Now when you create a wallet you will get a 12 word recovery phrase (no passphrase by default) to backup and keep safe.
##### ledger Nano S/X
: types of hardware wallets to store, send and receive crypto currencies
##### Nano 
: famous text GUI editor to start from commandline, not to be confused with Ledger Nano S/X, which is a cold storage.
##### Node
: A bitcoin full Node is a independent entity in a peer to peer ecosystem. A Node independently checks and verifies all protocol rules for incoming broadcasted transactions. A full node does not trust, but verifies. Technically speaking a *node* is a computer connected to other computers which follows rules and shares information. A *'full node'* is a computer in Bitcoin's peer-to-peer network which hosts and synchronises a copy of the entire Bitcoin blockchain. [Here](https://medium.com/@gloriazhao/map-of-the-bitcoin-network-c6f2619a76f3) is an excellent read on nodes, what they are and the differences between types of nodes.
##### Nodl
: A hardware box with to run a non-preloaded bitcoin node on it, [commercial site](https://www.nodl.it/). 
##### Output descriptors
: Descriptors are a clever way of importing specific keys into your node from any derivation, for any (or all) address types, single or multi signature, along with a fingerprint so offline psbt signers like a Coldcard and Fully Noded can sign the psbt if they hold the correct seed.
##### psbt
: Partially signed bitcoin transactions (PSBTs) Also covering BIP174. Partially Signed Bitcoin Transactions (PSBTs) are a data format that allows wallets and other tools to exchange information about a Bitcoin transaction and the signatures necessary to complete it.
##### pure bitcoin core wallets
: traditional bitcoin wallet, that has to be manually backed up, recovered etc using bitcoin-cli. Your node will sign transactions and will hold the private key.
##### rbf
: Replace-By-Fee (RBF) is a node policy that allows an unconfirmed transaction in a mempool to be replaced with a different transaction that spends at least one of the same inputs and which pays a higher transaction fee. **For newbies:** a transaction that can't get through because of too low fee, can be overridden (replaced) with a higher fee to maybe succeed instead.
##### RPC
: Remote Procedure Calls
##### segwit wrapped  bitcoin address (p2sh-p2wpkh) 
: BIP49 refers to the accepted common standard of deriving segwit "compatibility" addresses. These addresses begin with a 3.
##### Segwit addresses
: – Segregated Witness – or SegWit in short – reduced the transaction data’s size to allow for faster transactions, better scalability and decreased fees. Native SegWit (bech32) enhanced this even further and includes even lower fees. Not all exchanges and wallet providers support sending Bitcoin to a Native SegWit address yet, which is why you are presented both options in Ledger Live. Transactions between all 3 address types are possible
##### SSH
: Secure Shell (SSH) is a cryptographic network protocol for operating network services securely over an unsecured network.[1] Typical applications include remote command-line, login, and remote command execution, but any network service can be secured with SSH.
##### Standup app
: is a personal one-click Mac OS installer for Bitcoin Core and Tor that will present a QuickConnect QR code that can be used to pair mobile wallets for remote use over Tor V3. [Read more](https://github.com/BlockchainCommons/GordianSystem)
##### satoshi
: 0.000000001 BTC. A satoshi is the smallest unit of a bitcoin, equivalent to 100 millionth of a bitcoin.
##### signed raw transaction 
: [Wikipage](https://en.bitcoin.it/wiki/Raw_Transactions) explains it all
##### Trezor 
: a type of hardware wallet to store, send and receive crypto currencies
##### Tor
:Tor is free and open-source software for enabling anonymous communication. The name derived from the acronym for the original software project name "The Onion Router". [Read more in Wikipedia](https://en.wikipedia.org/wiki/Tor_(anonymity_network))
##### UTXO's
: Unspend transaction Outputs; UTXO stands for the unspent output from bitcoin transactions. Each bitcoin transaction begins with coins used to balance the ledger. UTXOs are processed continuously and are responsible for beginning and ending each transaction. Confirmation of transaction results in the removal of spent coins from the UTXO database. But a record of the spent coins still exists on the ledger. **for newbies**: UTXO is unspent bitcoin that you can "see" in your wallet and on the blockchain. It is an address and amount of sathosis. As soon as you spend the money, it won't add to your wallet balance anymore and therefore will only.


# Q&A section General

## What is Nodl?

It's a full node linked with a mobile wallet. (@Appelcline)

## What is the purpose of Nodl, why was it constructed?

GordianServer-macOS strives to provide the community with an easy-to-use "one-click" setup for a full node, complete with a purpose-built remote app for securely connecting to your node over Tor from anywhere in the world, providing you with a powerful suite of tools. (@ChristopherA)

## Why use Nodl?

There are a few advantages to this setup:

**Security**. A mobile wallet allows you to keep your private keys away from devices directly connected to the internet.

**Autonomy**. Maintaining your own full node ensures that you can't be censored, tracked, or otherwise taken advantage of by someone else. It ensures your self-sovereignty. (@Appelcline)


## What OSes can the Gordian System run on?

The Gordian server runs on MacOS, though the Bitcoin Standup technology that's at its foundation can also be run on UNIX machines, with the Linodes running Debian being particularly well tested.

The Gordian Wallets runs under iOS. (@Appelcline)

# Q&A section Userinterface

# Q&A section Nodl administrator

## How can I get to the Nodl administrator? 

# Q&A section Backup and Restore

## How does one restore your Nodl wallet when it has died?

# Q&A section Wallets

# Q&A section Connection

# Q&A section Node
