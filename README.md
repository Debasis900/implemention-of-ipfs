## Introduction
IPFS( [InterPlanetary File System](https://docs.ipfs.tech/concepts/what-is-ipfs/) ) is a **content-** **and** **identity-driven** hypermedia distribution **protocol.** It enables the creation of **fully** distributed **applications** and **thus** aims to make the web faster, **more** **secure** and more open.

IPFS is a distributed file system that aims to connect all computing devices to the same file system. In a way, this is similar to the original network targets, but IPFS is actually more like a single BitTorrent swarm exchanging Git objects. You can learn more about its origins in the article IPFS - Content Addressed, Versioned, P2P File System.

IPFS is becoming the new core subsystem of the Internet. Properly constructed, it can complement or replace the HTTP protocol.It can supplement or replace even more. 



https://github.com/Debasis900/implemention-of-ipfs/assets/33112583/0ddf37db-49a7-4d05-93a4-f97404a2b678


## How IPFS works
IPFS is a peer-to-peer (p2p) storage network. Content is available through partners around the world who can transmit information, store information, or both. IPFS knows how to find what you're asking for by the address of the content, not the location.

To Learn More about how IPFS works use [this](https://docs.ipfs.tech/concepts/how-ipfs-works/) link.

## Installation  
- To use the IPFS(InterPlanetary File System) first of all you have to install it. To download IPFS(CLI) Linux Binary run :
```shell
$ wget https://dist.ipfs.tech/kubo/v0.18.1/kubo_v0.181_linux-amd64.tar.gz
```

- Once the file is downloaded extract it.
```bash
$ tar -xvzf kubo_v0.18.1_linux-amd64.tar.gz
```

- Move into the kubo folder.
```bash
$ cd kubo
```

- Install the binary.
```bash
$ sudo bash install.sh
```

*Form more information use [this](https://docs.ipfs.tech/install/command-line/) link.*

*To get latest version of IPFS (CLI) Binary use [this](https://dist.ipfs.tech/#kubo) link*

*Note : To Install the GUI/Desktop Version use [this](https://docs.ipfs.tech/install/ipfs-desktop/) link and follow the instruction.*

## Post Installation 
---
- Once installation is done run the command below to initialize IPFS :
```bash
$ ipfs init
```

- This will create a **/.ipfs** folder in the home dir which contain all the important config files.

## Start the Server
---
- To start IPFS server run : 
```bash
$ ipfs daemon
```

- Once the server is active it will return a localhost IP(Web UI). That localhost IP is the web-client dashboard of IPFS which is very simple to use in its own.

## Uploading the File 
---
- To upload a file run : 
```bash
$ ipfs add <file name>
```
- The above action will return a Content Identifier or CID which is a unique value used to identify files stored on the IPFS network.

- Now share the CID with anyone you want.

## Downloading the File
---
- To download a file from IPFS network you need to have the CID and a fast internet service.

- Run : 
```bash
$ ipfs get <CID>
```
- Then a file will be downloaded with name same as the CID in the current dir.
- Once downloaded open the file in suitable application.

*Note : To learn more about IPFS use the [docs](https://docs.ipfs.tech/) which is very informative and  well documented.*
