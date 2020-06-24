# Cyphai

The problems solving and decision making model built by the Cyphai team comes from a wide range of experiences, formal and informal discussion and interactions between all Cyphai consultants and their counterparts (ranging from managers, students and parents looking for a solution to their day life or job activities).

The Cyphai model is a model from the research of a decision-making and problems solving specialist - Robert Michit - and his teams.

Using blockchain technology, it is possible to create contracts that offer a reward in exchange for a trained machine learning model for a particular database. This would allow users to train machine learning models and be rewarded via blockchain.

The Cyphai protocol will use the blockchain to automatically validate the solution, so there would be no debate as to whether the solution was correct or not. Users who submit solutions will have no risk of not being paid for their work. Contracts can be easily created by anyone with a database.

This creates a market where parties capable of solving machine learning problems can directly monetize their skills and where any organization or agent who has a problem to solve with AI can solicit solutions from developers around the world. This will encourage the creation of better learning models and make AI more accessible to companies.

For more information about Cyphai, please read the [white paper](https://cyph.ai/cyphai_whitepaper.pdf).

## Cyphai Contracts

The Cyphai contract can be found in the `contracts` directory.

## Requirements

To run the Cyphai unittests, we first need to setup our local development environment. The following commands have been tested for OSX and Linux.

### Installing the Solidity Compiler

### For Linux

***
sudo add-apt-repository ppa:ethereum/ethereum
sudo apt-get update
sudo apt-get install solc libssl-dev
***

### For OSX

Install a these homebrew packages:

***
brew install pkg-config libffi autoconf automake libtool openssl
***

Install the solidity compiler (solc):

***
brew update
brew upgrade
brew tap ethereum/ethereum
brew install solidity
brew link solidity
***

### Initialize your Virtual Environment

Install [virtualenv](https://virtualenv.pypa.io/en/stable/)

Setup a virtual environment with Python 3:

***
cd cyphai;
python3.6 -m venv venv;
source venv/bin/activate;

***

### Install the Populus Framework

Install `populus` and other requirements while in virtualenv:

***
pip install -r requirements.txt
***

You should be able to develop Ethereum contracts in Python 3 now

## Populus

All contracts are developed and tested using the Populus framework.

To compile all contracts, run the following:

***
populus compile
***

To run all the tests, use the following:

***
python -m pytest --disable-pytest-warnings tests/*
***
