# Getting Started with a Web 3 Aztec Protocol SDK Project
  
## Introduction

### The Purpose of this Learning Path is to document, or log, a Developer Journey   
The purpose of this tutorial repository is to provide a Web 3.0 Aztec Network getting started learning path for Web 2.0 developers who are new to working with Aztec technology and Web 3.0 in general.  

There are several screenshots in this tutorial. They are not necessarily applicable to your own personal developer path and experience - they are a general guide.  

### What is Aztec Network?  
Aztec is an open source layer 2 protocol (or network) which aims to bring scalability and privacy to Ethereum. It strives to enable affordable, private crypto payments via zero-knowledge proofs.  

### From the [Aztec Vision](https://aztec.network/vision) website  
  - [https://aztec.network/vision](https://aztec.network/vision)

Privacy isn't just a human right, it's a tool for creativity. With privacy by default, the world of games, NFTs, and DeFi applications just got bigger. Aztec is an open source layer 2 network that aims to bring scalability and privacy to Ethereum. It strives to enable affordable, private crypto payments via zero-knowledge proofs. Aztec is built from the ground up to be privacy-first. 

---

# Prerequisite steps: Begin Here

## Read the Aztec Protocol/Network Related Documentation

- ### Aztec Network Introduction  
  - [https://docs.aztec.network/](https://docs.aztec.network/)

- ### The Privacy Layer for Web3
  - [https://aztec.network/](https://docs.aztec.network/)

- ### An Introduction to Aztec
  - [https://medium.com/aztec-protocol/an-introduction-to-aztec-47c70e875dc7](https://medium.com/aztec-protocol/an-introduction-to-aztec-47c70e875dc7)
  
- ### The Aztec Programming SDK Overview
  - [https://docs.aztec.network/sdk/overview](https://docs.aztec.network/sdk/overview) 

- ### Aztec Protocol blog articles on Medium
  - [https://medium.com/aztec-protocol](https://medium.com/aztec-protocol) 

- ### Privacy Tech in Review: ZK Money
  - [https://medium.com/zero-knowledge-validator/privacy-tech-in-review-zk-money-efb59f879043](https://medium.com/zero-knowledge-validator/privacy-tech-in-review-zk-money-efb59f879043)

## Watch the Aztec Videos
- ### Aztec Talks and Videos
  - [https://docs.aztec.network/how-aztec-works/talks-videos](https://docs.aztec.network/how-aztec-works/talks-videos)

- ### Aztec 2.0 - A new layer 2 built with privacy at its core" - Joe Andrews
  - https://www.youtube.com/watch?v=ksmJahvYKSc

- ### Aztec - Joe Andrews (CPO) and Zac Williamson (CTO)
  - https://www.youtube.com/watch?v=NyBwdcIMT0M

- ### Privacy on blockchains and future of rollups | Joe from Aztec
  - [https://www.youtube.com/watch?v=3ZxyHTlkH9E](https://www.youtube.com/watch?v=3ZxyHTlkH9E)

---  

## Install Discord 
Discord will help you to communicate with the Aztec Network Developer Relations Engineering team.

- ### Aztec Network on Discord
  - [The Aztec Network Discord Channel](https://discord.gg/sJpr4KzjJa)

  - [Welcome to The Aztec Network Discord Channel](https://discord.com/channels/563037431604183070/945721017156898938)


- ### Discord Desktop Installation Guide
  - [https://support.discord.com/hc/en-us/articles/360034561191-Desktop-Installation-Guide](https://support.discord.com/hc/en-us/articles/360034561191-Desktop-Installation-Guide)

- ### Download Discord
  - [https://discord.com/download](https://discord.com/download)

---  

## Set up a MetaMask Wallet

- ### Install MetaMask for Chrome

  - [https://metamask.io/download/](https://metamask.io/download/)

<p align="center">
  <img width=auto height=auto src="screenshots/install-metamask-for-chrome.png">
</p>  

<p align="center">
  <img width=auto height=auto src="screenshots/metamask-setup-01.png">
</p>  

<p align="center">
  <img width=auto height=auto src="screenshots/metamask-setup-02.png">
</p>  

- ### How to set up an Ethereum wallet on MetaMask
  - [https://codehs.com/tutorial/jkeesh/how-to-set-up-an-ethereum-wallet-on-metamask](https://codehs.com/tutorial/jkeesh/how-to-set-up-an-ethereum-wallet-on-metamask)

---  

## How to set up the Aztec Mainnet Fork for Development  

### Please refer to the following  

- [The Aztec SDK Starter Repository](https://github.com/AztecProtocol/aztec-sdk-starter)

- [Aztec SDK Reference script](https://github.com/AztecProtocol/aztec-sdk-starter#aztec-sdk-reference-script)

- [Aztec SDK Requirements](https://github.com/AztecProtocol/aztec-sdk-starter#requirements)

- [Aztec SDK Development Environment](https://github.com/AztecProtocol/aztec-sdk-starter#environment)


### Use these details to configure the Aztec Mainnet Fork on your wallet  

- Network Name (recommended)  
```shell
Aztec Mainnet Fork
```

- RPC URL
```shell
https://mainnet-fork.aztec.network
```

- Chain ID
```shell
677868
```

- Currency Symbol  
```shell
ETH
```

- Rollup Provider URL
```shell
https://api.aztec.network/aztec-connect-testnet/falafel
```

- Block Explorer URL (optional)
```shell
https://aztec-connect-testnet-explorer.aztec.network
```

### Adding the Aztec Mainnet Fork to your MetaMask Wallet with the Chrome Web Extension    
  
<p align="center">
  <img width=500 height=auto src="screenshots/add-aztec-mainnet-fork-network-01-web.png">
</p>  

<p align="center">
  <img width=500 height=auto src="screenshots/add-aztec-mainnet-fork-network-02-web.png">
</p>  

### Adding the Aztec Mainnet Fork to your MetaMask Wallet with the Android Mobile App  
  
<p align="center">
  <img width=300 height=auto src="screenshots/add-aztec-mainnet-fork-network-01-mobile.png"> <img width=300 height=auto src="screenshots/add-aztec-mainnet-fork-network-02-mobile.png">
</p>  
<p align="center">
  <img width=300 height=auto src="screenshots/add-aztec-mainnet-fork-network-03-mobile.png"> <img width=300 height=auto src="screenshots/add-aztec-mainnet-fork-network-04-mobile.png">
</p>  

---
  
## Building the Aztec SDK Starter Code on macOS and Linux  

These notes record steps that were performed **on a macOS development laptop** and a **Linux (Ubuntu) development laptop**.  

Other operating systems should have similar options to enable the equivalent operations.  

I use the [Homebrew](https://brew.sh/) package manager on my macOS development laptop.

Package managers like [Homebrew for macOS](https://brew.sh/) have equivalents such as [Chocolatey for Windows](https://chocolatey.org/) and many others for Linux.  

Here is a list of software package management systems:
  - [https://en.wikipedia.org/wiki/List_of_software_package_management_systems](https://en.wikipedia.org/wiki/List_of_software_package_management_systems)

---  

### Read/refer to these resources  

- Aztec Network Introduction 
  - [https://docs.aztec.network/](https://docs.aztec.network/) 
- `@aztec/sdk` and `@aztec/bridge-clients` Documentation and NPM Packages
  - [https://developers.aztec.network/](https://developers.aztec.network/)
  - [https://www.npmjs.com/package/@aztec/sdk](https://www.npmjs.com/package/@aztec/sdk)
  - [https://www.npmjs.com/package/@aztec/bridge-clients](https://www.npmjs.com/package/@aztec/bridge-clients)
- The Aztec SDK Overview
  - [https://docs.aztec.network/sdk/overview](https://docs.aztec.network/sdk/overview)
- The Aztec SDK Starter Repository
  - [https://github.com/AztecProtocol/aztec-sdk-starter](https://github.com/AztecProtocol/aztec-sdk-starter)

---  

### Install the SDK starter runtime dependencies

  - [https://github.com/critesjosh/aztec-sdk-starter#requirements](https://github.com/critesjosh/aztec-sdk-starter#requirements)
  - [https://github.com/AztecProtocol/aztec-sdk-starter#requirements](https://github.com/AztecProtocol/aztec-sdk-starter#requirements)

For your reference; How to install [Homebrew](https://brew.sh/), NodeJS and NPM on macOS   

  - [https://medium.com/@hayasnc/how-to-install-nodejs-and-npm-on-mac-using-homebrew-b33780287d8f](https://medium.com/@hayasnc/how-to-install-nodejs-and-npm-on-mac-using-homebrew-b33780287d8f)

I already have Homebrew on my macOS system, so I will proceed with installing NodeJS, NPM and Yarn.  
  
```shell
$ cd ~

# -- Node
$ brew install node
$ brew info node
$ brew info npm

# -- Yarn
$ brew install yarn
$ brew info yarn
```  
  
<p align="center">
  <img width=auto height=auto src="screenshots/brew-info-node.png">
</p>  

<p align="center">
  <img width=auto height=auto src="screenshots/brew-info-yarn.png">
</p>  

On Linux (Debian/Ubuntu distributions), do the following.

```shell
$ cd ~
$ sudo apt-get install -y build-essential
$ curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash - && sudo apt-get install -y nodejs
$ sudo npm install -g npm
$ which node
$ which npm
$ node -v
$ npm -v
```
<p align="center">
  <img width=auto height=auto src="screenshots/linux-node-npm-versions.png">
</p>  

Ensure that TypeScript and its dependencies are installed.  

```shell
$ npm install ts-node --save-dev
$ npm install typescript -g
$ npm install typescript --save-dev
```  
<p align="center">
  <img width=auto height=auto src="screenshots/typescript-setup-01.png">
</p>  

On Linux.

```shell
$ sudo npm install ts-node --save-dev
$ sudo npm install typescript -g
$ sudo npm install typescript --save-dev
```
---  

### Clone the SDK starter repository from GitHub  
  
```shell
$ mkdir AztecProtocol
$ cd AztecProtocol
$ git clone https://github.com/AztecProtocol/aztec-sdk-starter.git
$ cd aztec-sdk-starter
$ ls -al
```  
  
<p align="center">
  <img width=auto height=auto src="screenshots/aztec-sdk-starter-ls.png">
</p>  

---

### Install the SDK starter package dependencies

On macOS.

```shell
$ yarn
```  
  
Be sure to pick the highest, most recent, version number of `@aztec/bridge-clients`.  

<p align="center">
  <img width=auto height=auto src="screenshots/aztec-sdk-starter-dependencies-01.png">
</p>

<p align="center">
  <img width=auto height=auto src="screenshots/aztec-sdk-starter-dependencies-02.png">
</p>

<p align="center">
  <img width=auto height=auto src="screenshots/aztec-sdk-starter-dependencies-03.png">
</p>

On Linux.

```shell
$ yarn
```  
<p align="center">
  <img width=auto height=auto src="screenshots/linux-yarn-install1.png">
</p>

<p align="center">
  <img width=auto height=auto src="screenshots/linux-yarn-install2.png">
</p>

Also make sure to periodically check for updates to the repository and dependencies.  

```shell
$ git pull
$ yarn upgrade --latest
```  

Yarn upgrade on Linux.

<p align="center">
  <img width=auto height=auto src="screenshots/linux-yarn-upgrade1.png">
</p>

---

### Create and configure the SDK Environment File and run the SDK Setup Script

Refer to the following section of the SDK starter repository documentation.
- [https://github.com/AztecProtocol/aztec-sdk-starter#run](https://github.com/AztecProtocol/aztec-sdk-starter#run)

Remain inside the root directory of your local (cloned) `aztec-sdk-starter` repository and copy the provided example environment script, `.env.example`, in order to create a `.env` file.

```shell
$ cp .env.example .env
$ ls -al .env*
$ cat .env
```  
  
<p align="center">
  <img width=auto height=auto src="screenshots/aztec-sdk-starter-env.png">
</p>  
  
Edit your new `.env` file and add your Ethereum private key or mnemonic. 
- DO NOT DISCLOSE THIS TO ANYONE!
- NEVER PUSH THE `.env` FILE TO ANY PUBLIC REPOSITORY! 
- The local Git repository `.gitignore` file should have an exclusion entry for `.env`.  
  
Now run the `./src/latest/index.ts` SDK setup script.

```shell
$ yarn go
```  


---

## General Web 3.0 References
- CryptoCurrency Wiki 
  - [https://cryptocurrencywiki.org/Main_Page](https://cryptocurrencywiki.org/Main_Page)
- Blockchain and CryptoCurrency Wiki 
  - [https://golden.com/wiki/Blockchain_and_cryptocurrency-8AR86E6](https://golden.com/wiki/Blockchain_and_cryptocurrency-8AR86E6) 
- Ethereum Development Documentation
  - [https://ethereum.org/en/developers/docs/](https://ethereum.org/en/developers/docs/)
- Ethereum Stack Exchange  
  - [https://ethereum.stackexchange.com/](https://ethereum.stackexchange.com/)

---

## Aztec Connect/Protocol Resources
- Aztec Testnet Version of zk.money 
  - [https://aztec-connect-testnet.zk.money/](https://aztec-connect-testnet.zk.money/)
- Aztec Testnet Server Status 
  - [https://api.aztec.network/aztec-connect-testnet/falafel/status](https://api.aztec.network/aztec-connect-testnet/falafel/status)
- Aztec Testnet Block Explorer 
  - [https://aztec-connect-testnet-explorer.aztec.network/](https://aztec-connect-testnet-explorer.aztec.network/)
- The Aztec Noir Programming Language 
  - [https://github.com/noir-lang/noir](https://github.com/noir-lang/noir)
- Aztec Network Introduction
  - [https://docs.aztec.network/](https://docs.aztec.network/)
- `@aztec/sdk` and `@aztec/bridge-clients` Documentation and NPM Packages
  - [https://developers.aztec.network/](https://developers.aztec.network/)
  - [https://www.npmjs.com/package/@aztec/sdk](https://www.npmjs.com/package/@aztec/sdk)
  - [https://www.npmjs.com/package/@aztec/bridge-clients](https://www.npmjs.com/package/@aztec/bridge-clients)
- The Aztec SDK Starter Repository
  - [https://github.com/critesjosh/aztec-sdk-starter](https://github.com/critesjosh/aztec-sdk-starter)

---


#### LICENSE for this content

**[MIT License](https://opensource.org/licenses/MIT)**

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

