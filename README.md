# Cyphai

The problems solving and decision making model built by the Cyphai team comes from a wide range of experiences, formal and informal discussion and interactions between all Cyphai consultants and their counterparts (ranging from managers, students and parents looking for a solution to their day life or job activities).

The Cyphai model is a model from the research of a decision-making and problems solving specialist - Robert Michit - and his teams.

The Cyphai protocol utilizes blockchain technology via smart contracts. The contract allows anyone to post a database, an evaluation function, and a monetary reward for anyone who can provide the best trained machine learning model for the data. Participants train deep neural networks to model the data, and submit their trained networks to the blockchain. The blockchain executes these neural network models to evaluate submissions, and ensure that payment goes to the best model.

The contract allows for the creation of a decentralized and trustless marketplace for exchanging ML models and many more under development. This gives ML practitioners an opportunity to monetize their skills directly. It also allows any participant or organization to solicit machine learning models from all over the world. This will incentivize the creation of better machine learning models, and make AI more accessible to companies and software agents. Anyone with a database, including software agents can create Cyphai contracts.

[Whitepaper](https://cyph.ai)

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

## Cyphai Contracts

The Cyphai contract can be found in the `contracts` directory.

For more information about Cyphai contracts, please read the [white paper](#).
