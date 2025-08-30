# ⭐️ A proxy scraper made using Protractor | Proxy list - Updates every hours 🔥

[![Every 10 Minutes Update](https://github.com/Skiddle-ID/proxylist/actions/workflows/nodejs.yml/badge.svg?branch=master)](https://github.com/Skiddle-ID/proxylist/actions/workflows/nodejs.yml)
![GitHub](https://img.shields.io/github/license/Skiddle-ID/proxylist)
![GitHub last commit](https://img.shields.io/github/last-commit/Skiddle-ID/proxylist)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Skiddle-ID/proxylist/graphs/commit-activity)
[![Website sunny9577.github.io](https://img.shields.io/website-up-down-green-red/http/github.io.svg)](https://sunny9577.github.io/)
[![made-with-nodejs](https://img.shields.io/badge/Made%20with-Nodejs-green.svg)](https://www.nodejs.org/)

<!-- dynamic-count-start -->
## Current Proxy Count: 1400+ 🚀
<!-- dynamic-count-end -->


## Quick Access - By Format


TXT

    curl "https://skiddle-id.github.io/proxylist/proxies.txt" > proxies.txt

JSON

    curl "https://skiddle-id.github.io/proxylist/proxies.json" > proxies.json

CSV

    curl "https://skiddle-id.github.io/proxylist/proxies.csv" > proxies.csv

YAML


    curl "https://skiddle-id.github.io/proxylist/proxies.yaml" > proxies.yaml

XML


    curl "https://skiddle-id.github.io/proxylist/proxies.xml" > proxies.xml

## Quick Access - By Type
###### Supported formats: txt | json | csv | yaml | xml

SOCKS5

    curl "https://skiddle-id.github.io/proxylist/generated/socks5_proxies.txt" > socks5_proxies.txt


SOCKS4

    curl "https://skiddle-id.github.io/proxylist/generated/socks4_proxies.txt" > socks4_proxies.txt

HTTP(S)

    curl "https://skiddle-id.github.io/proxylist/generated/http_proxies.txt" > http_proxies.txt


## Setup Requirements
1 - A Windows, Mac or Linux Computer

2 - Google Chrome installed

3 - Nodejs and NPM installed

## Setup
This bot is based on [protractor](https://www.protractortest.org/#/) automated browser testing software.
### 1 - Open a terminal and make sure you are in the project directory
	cd proxy-scraper

### 2 - Make sure you have protractor installed
To check if you have protractor installed run:

	protractor --version

If the output is something like this:

	Version 7.0.0

This means protractor is already installed, otherwise run the command:

	npm install -g protractor

### 3 - Install Selenium Webdriver
This is where your program will run, to install it simply execute the command:

	webdriver-manager

### 4 - Database Connectivity ( Only if u want to save output to database)
You can skip this step just set SAVE_TO_DB to false in config.js

Go to the file config.js and change with your login information

	npm install mysql2
	
Table Structure (Table Name: proxies_tb)
		
|Name|Type|Collation|Attributes|Null|Default|Comments|Extra|
|----|----|---------|----------|----|-------|--------|-----|
|1	|idPrimary	|int(11)	|		|No	|None		|AUTO_INCREMENT
|2	|proxyIndex	|varchar(50)	|latin1_swedish_ci		|No	|None		
|3	|port	|int(10)		|	|No	|None		
|4	|country	|varchar(100)	|latin1_swedish_ci		|No	|None		
|5	|type	|varchar(100)	|latin1_swedish_ci		|No	|None		
|6	|anonymity	|varchar(100)	|latin1_swedish_ci		|No	|None	

## Running the bot

### 1 - Update the Selenium webserver and install dependencies
Open a terminal and make sure you are in the project directory:
	
	cd proxy-scraper
	
Update webdrivers:

	webdriver-manager update
	
Install dependencies:

	npm install
	
### 2 - Run the bot
Its time to start retrieving the proxies, make sure you are in the project directory:
	
	cd proxy-scraper
	
Run the bot:

	protractor conf.js

## Additional Tools

- #### socks5_test.py
	
	This python script tests the SOCKS5 proxies against https://icanhazip.com and https://eset.com. Contributed by [@techroy23](https://www.github.com/techroy23)

	Steps to run:
	- pip3 install tabulate pysocks
	- python3 socks5_test.py

## Disclaimer
This repository is intended solely for educational purposes. I neither endorse nor encourage any illegal activities or behavior.

[![Stargazers over time](https://starchart.cc/Skiddle-ID/proxylist.svg)](https://starchart.cc/Naereen/badges)

---
<!-- License + Copyright -->
<p  align="center">
  <i>© <a href="https://skiddle.id">Skiddle ID</a> 2025</i><br>
  <i>Licensed under <a href="https://gist.github.com/arcestia/dc2bef037daf25773cb972b69d22be09">MIT</a></i>
</p>
