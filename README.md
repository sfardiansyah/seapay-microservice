# Seapay

Seapay is a fintech app consists of 4 different services

- [Description](#description)
- [How to Use](#how-to-use)
  - [Installation](#installation)
    - [Linux](#installation-for-linux)
    - [Mac](#installation-for-mac)
  - [Usage](#how-to-use)
    - [How to Build](#how-to-build)
    - [How to Run](#how-to-run)

### Description

- API gateway
  - API gateway service routes all requests to other services
- User account
  - User account service takes care of user management: user creation, get user data, etc
- Wallet
  - Wallet service handles all wallet functionalities: update balance, get balance, create wallet, etc
- Transaction
  - Transaction service manage all transaction data

The project itself has 4 modules

- seapay-api
  - a module that abstracts interface for all services
- seapay-common
  - a module that groups all common functionalities used by all services
- seapay-domain
  - the bussiness logic for all services goes here
- seapay-monolith
  - an entry point of our monolithic app, including all handlers

# Installation

### Installation for Linux

- [Install PostgreSQL](https://tecadmin.net/install-postgresql-server-on-ubuntu/)
- [Install Java](https://thishosting.rocks/install-java-ubuntu/)
- [Install Postman](https://www.getpostman.com/)

### Installation for Mac

- [Install PostgreSQL](https://www.robinwieruch.de/postgres-sql-macos-setup/)
- Install Java

```
brew cask install java
```

- [Install Postman](https://www.getpostman.com/)

# Usage

### How to Build

```
make all
```

### How to Run

```
make run
```
