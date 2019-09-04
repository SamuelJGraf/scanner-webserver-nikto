---
title: "Nikto"
path: "scanner/Nikto"
category: "scanner"
usecase: "Webserver Vulnerability Scanner"
release: "https://img.shields.io/github/release/secureCodeBox/scanner-webserver-nikto.svg"

---

Nikto is a free software command-line vulnerability scanner that scans webservers for dangerous files/CGIs, outdated server software and other problems. It performs generic and server type specific checks. It also captures and prints any cookies received. 

<!-- end -->

# About

This repository contains a self contained µService utilizing the Nikto scanner for the secureCodeBox project.

Further Documentation:

- [Project Description][scb-project]
- [Developer Guide][scb-developer-guide]
- [User Guide][scb-user-guide]

## Configuration Options

To configure this service specify the following environment variables:

| Environment Variable       | Value Example |
| -------------------------- | ------------- |
| ENGINE_ADDRESS             | http://engine |
| ENGINE_BASIC_AUTH_USER     | username      |
| ENGINE_BASIC_AUTH_PASSWORD | 123456        |

## Development

### Local setup

1. Clone the repository
2. You might need to install some dependencies `gem install sinatra rest-client`
3. Run locally `ruby src/main.rb`

### Test

To run the testsuite run:

`rake test`

### Build

To build the docker container run:

`docker build -t CONTAINER_NAME .`


[![Build Status](https://travis-ci.com/secureCodeBox/scanner-webserver-nikto.svg?branch=develop)](https://travis-ci.com/secureCodeBox/scanner-webserver-nikto)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![GitHub release](https://img.shields.io/github/release/secureCodeBox/scanner-webserver-nikto.svg)](https://github.com/secureCodeBox/scanner-webserver-nikto/releases/latest)


[scb-project]: https://github.com/secureCodeBox/secureCodeBox
[scb-developer-guide]: https://github.com/secureCodeBox/secureCodeBox/blob/develop/docs/developer-guide/README.md
[scb-developer-guidelines]: https://github.com/secureCodeBox/secureCodeBox/blob/develop/docs/developer-guide/README.md#guidelines
[scb-user-guide]: https://github.com/secureCodeBox/secureCodeBox/tree/develop/docs/user-guide
