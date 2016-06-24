---
layout: post
title:  "Node On Linux"
date:   2015-04-28
categories: Linux

---

Node.js
=======
Node.js is a JavaScript-based framework/platform used to develop I/O intensive web applications. Being open source, completely free, anyone can contribute and be a part of it.

NPM
====
NVM acts as a packet manager for node. It provides online repositories for node.js projects, facilitates command line interface for the installation of Node.js packages, version management and dependency management.<br>
Installation can be done using following commands:

* For installing packages <br>
  npm install async 

* For installing dependencies <br>
  npm install

* For installing modules <br>
  npm install <module name>

NVM
====
NVM supports version management of node.js versions. It is a simple bash script that provides the functionality of quickly switching to other versions of node.js.<br>
NVM can be installed using following steps:


1. Updating the packages already present<br>
   sudo apt-get update  


2. Installing the build essential packages <br>
   sudo apt-get install build-essential libssl-dev


3. Installing NVM <br>
   curl https://raw.githubusercontent.com/creationix/nvm/v0.25.0/install.sh | bash

4. Once this is done, close and restart the terminal and add the following command<br>
   source ~/.profile

Node version
=============
* To check the node versions present on your machine <br>
  nvm ls

* To switch to a particular version <br>
  nvm use <-version->


_______________________________________________________________________________________________________________________________________________________
