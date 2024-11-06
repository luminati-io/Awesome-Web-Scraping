# Python Web Scraping

This document contains a list of libraries and resources for web scraping in Python.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [HTTP Clients](#http-clients)
    - [WebSockets](#websockets)
    - [Low Level](#low-level)
  - [Parsers](#parsers)
    - [HTML/XML Parsers](#htmlxml-parsers)
    - [URL Parsers](#url-parsers)
    - [CSV Parsers](#csv-parsers)
    - [Text Parsers](#text-parsers)
    - [Date and Time Parsers](#date-and-time-parsers)
    - [PDF Parsers](#pdf-parsers)
    - [HTTP Parsers](#http-parsers)
    - [Email Parsers](#email-parsers)
    - [Markdown Parsers](#markdown-parsers)
    - [YAML Parsers](#yaml-parsers)
    - [SQL Parsers](#sql-parsers)
    - [Office File Parsers](#office-file-parsers)
    - [Other](#other)
  - [Web Scraping](#web-scraping)
    - [Frameworks](#frameworks)
    - [Tools and Plugins](#tools-and-plugins)
    - [Anti-Bot Bypass](#anti-bot-bypass)
    - [Proxy Integration](#proxy-integration)
    - [CAPTCHA Solving](#captcha-solving)
    - [User-Agent Spoofing](#user-agent-spoofing)
    - [Scraper Management](#scraper-management)
  - [Web Automation](#web-automation)
    - [Browser Automation Frameworks](#browser-automation-frameworks)
    - [Tools and Plugins](#tools-and-plugins-1)
    - [Other](#other-1)
  - [Data Export](#data-export)
    - [JSON](#json)
    - [CSV](#csv)
    - [Other](#other-2)
  - [Data Processing](#data-processing)
    - [Character Encoding](#character-encoding)
    - [Date and Time](#date-and-time)
    - [Prices](#prices)
    - [Human Names](#human-names)
    - [Phone Numbers](#phone-numbers)
    - [Slugs](#slugs)
    - [URLs and Network Addresses](#urls-and-network-addresses)
    - [Languages](#languages)
  - [Other](#other-3)
    - [Multiprocessing](#multiprocessing)
    - [Task Scheduling](#task-scheduling) 
- [Popular Web Scraping Stacks](#popular-web-scraping-stacks)
  - [Static Web Pages](#static-web-pages)
  - [Dynamic Web Pages](#dynamic-web-pages)
- [Guides and Tutorials](#guides-and-tutorials)
  - [General Guides](#general-guides)
  - [Proxies](#proxies)
  - [User Agent Setting](#user-agent-setting)
  - [Parsing](#parsing)
  - [Scraping Popular Sites](#scraping-popular-sites)
  - [Anti-Bot Bypass](#anti-bot-bypass-1)
  - [Comparisons](#comparisons)

## Libraries
**Note**: All selected libraries are actively maintained and compatible with Python 3+.

### Network

#### HTTP Clients

- [requests](https://github.com/kennethreitz/requests): A simple, yet elegant HTTP library
- [httpx](https://github.com/encode/httpx): A next generation HTTP client for Python
- [aiohttp](https://github.com/aio-libs/aiohttp): An asynchronous HTTP client/server framework for [asyncio](https://docs.python.org/3/library/asyncio.html) and Python
- [uplink](https://github.com/prkumar/uplink): A declarative HTTP Client for Python
- [grequests](https://github.com/spyoungtech/grequests): A library to use Requests with Gevent to make asynchronous HTTP Requests easily
- [treq](https://github.com/twisted/treq): Python requests like API built on top of Twisted's HTTP client
- [pycurl](https://github.com/pycurl/pycurl): A Python interface to [libcurl](http://curl.haxx.se/libcurl/)
- [urllib3](https://github.com/shazow/urllib3): A user-friendly HTTP client library for Python
- [httplib2](https://github.com/httplib2/httplib2): A small, fast HTTP client library for Python. It features persistent connections, cache, and Google App Engine support. Originally written by Joe Gregorio, now supported by the community
- [urllib](https://docs.python.org/3/library/urllib.html): A Python Standard Library module for dealing with network requests

#### WebSockets

- [websockets](https://github.com/python-websockets/websockets): A library for building WebSocket servers and clients in Python
- [websocket-client](https://github.com/websocket-client/websocket-client): A WebSocket client for Python
- [AutobahnPython](https://github.com/tavendo/AutobahnPython): WebSocket and WAMP in Python for [Twisted](https://github.com/twisted/twisted) and asyncio
- [WebSocket-for-Python](https://github.com/Lawouach/WebSocket-for-Python): A WebSocket client and server library for Python 2 and 3 as well as PyPy (ws4py 0.5.1)
- [simple-websocket](https://github.com/miguelgrinberg/simple-websocket): A simple WebSocket server and client for Python
- [wsproto](https://github.com/python-hyper/wsproto): A Sans-IO WebSocket protocol implementation

#### Low Level

- [dpkt](https://github.com/kbandla/dpkt): Fast, simple packet creation / parsing, with definitions for the basic TCP/IP protocols
- [pyopenssl](https://github.com/pyca/pyopenssl): A Python wrapper around the OpenSSL library
- [scapy](https://github.com/secdev/scapy): A Python-based interactive packet manipulation program & library
- [impacket](https://github.com/SecureAuthCorp/impacket/): A collection of Python classes for working with network protocols
- [socket](https://docs.python.org/3/library/socket.html): A Python Standard library module that provides access to the BSD socket interface

### Parsers

#### HTML/XML Parsers

- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/): A program designed for screen-scraping HTML [**[Beautiful Soup Proxy Integration](https://brightdata.com/integration/beautifulsoup)**]
- [lxml](https://github.com/lxml/lxml/): A feature-rich and easy-to-use library for processing XML and HTML in the Python language
- [pyquery](https://github.com/gawel/pyquery): A jquery-like library for Python to perfrom queries on XML and HTML documents
- [html5lib](https://github.com/html5lib/html5lib-python): A Standards-compliant library for parsing and serializing HTML documents and fragments in Python
- [parsel](https://github.com/scrapy/parsel): A library that lets you extract data from XML/HTML documents using XPath or CSS selectors
- [xmltodict](https://github.com/martinblech/xmltodict): A Python module that makes working with XML feel like you are working with JSON
- [untangle](https://github.com/stchris/untangle): A library to convert XML to Python objects
- [selectolax](https://github.com/rushter/selectolax): Python binding to Modest and Lexbor engines (fast HTML5 parser with CSS selectors)
- [html5-parser](https://github.com/kovidgoyal/html5-parser): A fast C-based HTML 5 parsing library for Python
- [html.parser](https://docs.python.org/3/library/html.parser.html): A Python Standard Library module that serves as the basis for parsing text files formatted in HTML (HyperText Mark-up Language) and XHTML

#### URL Parsers

- [urllib.parse](https://docs.python.org/3/library/urllib.parse.html): A Python Standard Library module to parse URLs into components
- [furl](https://github.com/gruns/furl): A Python library that makes URL parsing and manipulation easy
- [purl](https://github.com/codeinthehole/purl): A simple, immutable URL class with a clean API for interrogation and manipulation
- [micawber](https://github.com/coleifer/micawber): A small library for extracting rich content from URLs

#### CSV Parsers

- [CleverCSV](https://github.com/alan-turing-institute/CleverCSV): A Python package for handling messy CSV files

#### Text Parsers

- [textract](https://github.com/deanmalmgren/textract): A library to extract text from any document
- [rows](https://github.com/turicas/rows): A common, beautiful interface to tabular data, no matter the format

#### Date and Time Parsers

- [dateparser](https://github.com/scrapinghub/dateparser): A Python parser for human readable dates
- [ciso8601](https://github.com/closeio/ciso8601): A fast ISO8601 date time parser for Python written in C

#### PDF Parsers

- [PyPDF2](https://github.com/mstamy2/PyPDF2): A pure-python PDF library capable of splitting, merging, cropping, and transforming the pages of PDF files
- [pdftables](https://pypi.python.org/pypi/pdftables) - Extract tables from PDF files directly
- [PyMuPDF](https://github.com/pymupdf/PyMuPDF): A high performance Python library for data extraction, analysis, conversion & manipulation of PDF (and other) documents

#### HTTP Parsers

- [httptools](https://github.com/MagicStack/httptools): A Python binding for the nodejs HTTP parser
- [http-parser](https://github.com/benoitc/http-parser): An HTTP request/response parser for python in C

#### Email Parsers

- [flanker](https://github.com/mailgun/flanker): A Python email address and Mime parsing library

#### Markdown Parsers

- [Python-Markdown](https://github.com/waylan/Python-Markdown): A Python implementation of John Gruber's Markdown with Extension support
- [mistune](https://github.com/lepture/mistune): A fast yet powerful Python Markdown parser with renderers and plugins
- [python-frontmatter](https://github.com/eyeseast/python-frontmatter): A library to parse and manage posts with YAML (or other) frontmatter
- [markdown2](https://github.com/trentm/python-markdown2): A fast and complete implementation of Markdown in Python

#### YAML Parsers

- [PyYAML](https://github.com/yaml/pyyaml): A full-featured YAML processing framework for Python

#### SQL Parsers

- [sqlparse](https://sqlparse.readthedocs.org/): A non-validating SQL parser.
- [sqlglot](https://github.com/tobymao/sqlglot): A Python SQL parser and transpiler

#### Office File Parsers

- [python-docx](https://github.com/python-openxml/python-docx): A library to create and modify Word documents with Python
- [XlsxWriter](https://github.com/jmcnamara/XlsxWriter): A Python module for creating Excel XLSX files

#### Other

- [feedparser](https://github.com/kurtmckee/feedparser): A library to parse Atom and RSS feeds in Python
- [rss-parser](https://github.com/dhvcc/rss-parser): A typed python RSS parsing module built using xmltodict and pydantic
- [reppy](https://github.com/seomoz/reppy): A modern robots.txt parser for Python
- [ultimate-sitemap-parser](https://github.com/GateNLP/ultimate-sitemap-parser): A website sitemap parser that supports all sitemap formats
- [psd-tools](https://github.com/kmike/psd-tools): A Python package for reading Adobe Photoshop PSD files
- [chompjs](https://github.com/Nykakin/chompjs): A library to parse JavaScript objects into Python data structures
- [xhtml2pdf](https://github.com/xhtml2pdf/xhtml2pdf): A library for converting HTML into PDFs using ReportLab
- [html2text](https://github.com/Alir3z4/html2text): A library to convert HTML to Markdown-formatted text

### Web Scraping

#### Frameworks

- [scrapy](https://github.com/scrapy/scrapy): A fast high-level web crawling & scraping framework for Python [**[Scrapy Proxy Integration](https://brightdata.com/integration/scrapy)**]
- [autoscraper](https://github.com/alirezamika/autoscraper): A smart, automatic, fast and lightweight web scraper for Python
- [requests-html](https://github.com/psf/requests-html): A library that intends to make parsing HTML (e.g. scraping the web) as simple and intuitive as possible
- [ruia](https://github.com/howie6879/ruia): An Async Python 3.6+ web scraping micro-framework based on asyncio
- [gazpacho](https://github.com/maxhumber/gazpacho/): A simple, fast, and modern web scraping library
- [dude](https://github.com/roniemartinez/dude): A simple framework for writing web scrapers using Python decorators
- [mechanize](https://github.com/python-mechanize/mechanize): A library for automating interaction with HTTP web servers

#### Tools and Plugins

- [cssselect](https://github.com/scrapy/cssselect): A BSD-licensed Python library to parse CSS3 selectors and translate them to XPath 1.0 expressions
- [scrapy-splash](https://github.com/scrapy-plugins/scrapy-splash): Scrapy+Splash for JavaScript integration
- [jusText](https://github.com/miso-belica/jusText): A tool for removing boilerplate content, such as navigation links, headers, and footers from HTML pages
- [extruct](https://github.com/scrapinghub/extruct): A library to extract embedded metadata from HTML markup
- [htmldate](https://github.com/adbar/htmldate): A fast and robust date extraction from web pages, with Python or on the command line
- [lassie](https://github.com/michaelhelmick/lassie): A Python library for retrieving basic content from websites
- [youtube-dl](http://rg3.github.io/youtube-dl/): A Command-line program to download videos from YouTube.com and other video sites
- [dragnet](https://github.com/dragnet-org/dragnet): A web page content extraction
- [extractnet](https://github.com/currentsapi/extractnet): A fork of Dragnet that also extract author, headline, date, keywords from context, as well as built in metadata extraction all in one package

#### Anti-Bot Bypass

- [cloudscraper](https://github.com/venomous/cloudscraper): A Python module to bypass Cloudflare's anti-bot page
- [curl-impersonate](https://github.com/lwthiker/curl-impersonate): A special build of curl that can impersonate Chrome & Firefox

#### Proxy Integration
- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports  state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]

#### CAPTCHA Solving
- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver
that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]
- [captcha_solver](https://github.com/lorien/captcha_solver): An Universal python API to captcha solving services
- [python-anticaptcha](https://github.com/ad-m/python-anticaptcha): A client library for solve captchas with Anticaptcha.com support
- [unicaps](https://github.com/sergey-scat/unicaps): A unified Python API for CAPTCHA solving services
- [python3-anticaptcha](https://github.com/AndreiDrang/python3-anticaptcha): A Python library for AntiCaptcha

#### User-Agent Spoofing

- [fake-useragent](https://github.com/fake-useragent/fake-useragent): An up-to-date simple useragent faker with real world database
- [python-user-agents](https://github.com/selwin/python-user-agents): A Python library that provides an easy way to identify devices like mobile phones, tablets and their capabilities by parsing (browser) user agent strings
- [user_agent](https://github.com/lorien/user_agent): A generator of the User-Agent header

#### Scraper Management

- [Gerapy](https://github.com/Gerapy/Gerapy): A distributed crawler management framework based on Scrapy, Scrapyd, Django and Vue.js
- [scrapydweb](https://github.com/my8100/scrapydweb): A web app for Scrapyd cluster management, Scrapy log analysis & visualization, auto packaging, timer tasks, monitor & alert, and mobile UI

### Web Automation

#### Browser Automation Frameworks

- [selenium](https://github.com/SeleniumHQ/selenium): A browser automation framework and ecosystem
- [playwright](https://github.com/microsoft/playwright-python): A Python version of the Playwright testing and automation library
- [pyppeteer](https://github.com/pyppeteer/pyppeteer): A headless Chrome/Chromium automation library (unofficial port of [Puppeteer](https://pptr.dev/))
- [seleniumbase](https://github.com/seleniumbase/SeleniumBase): A Python's all-in-one framework for web crawling, scraping, testing, and reporting. Supports pytest. UC Mode provides stealth. Includes many tools
- [splash](https://github.com/scrapinghub/splash): A lightweight, scriptable browser as a service with an HTTP API
- [crawlee](https://github.com/apify/crawlee-python): A web scraping and browser automation library for Python to build reliable crawlers. Extract data for AI, LLMs, RAG, or GPTs. Download HTML, PDF, JPG, PNG, and other files from websites. Works with BeautifulSoup, Playwright, and raw HTTP. Both headful and headless mode. With proxy rotation
- [botasaurus](https://github.com/omkarcloud/botasaurus): An all-in-one framework to build awesome scrapers
- [splinter](https://github.com/cobrateam/splinter): A Python test framework for web applications
- [MechanicalSoup](https://github.com/hickford/MechanicalSoup): A Python library for automating interaction with websites

#### Tools and Plugins

- [requestium](https://github.com/tryolabs/requestium): An integration layer between Requests and Selenium for automation of web actions
- [playwright_stealth](https://github.com/AtuboDad/playwright_stealth): A Python port of the [puppeteer-extra-plugin-stealth](https://github.com/berstend/puppeteer-extra/tree/master/packages/puppeteer-extra-plugin-stealth) plugin
- [pyppeteerstealth](https://github.com/dgtlmoon/pyppeteerstealth): Pyppeteer stealth plugin to attempt to look like a normal browser

#### Other

- [ninjemail](https://github.com/david96182/ninjemail): A Python library for automated email account creation. Create multiple accounts easily with support for major email providers

### Data Export

#### JSON

- [json](https://docs.python.org/3/library/json.html): A Python Standard Library module to encode and decode JSON data
- [orjson](https://github.com/ijl/orjson): A fast, correct Python JSON library supporting dataclasses, datetimes, and [NumPY](https://numpy.org/)
- [ujson](https://github.com/esnme/ultrajson): An ultra fast JSON decoder and encoder written in C with Python bindings

#### CSV

- [csv](https://docs.python.org/3/library/csv.html): A Python Standard Library module for CSV file reading and writing

#### Other

- [msgspec](https://github.com/jcrist/msgspec) - A fast serialization and validation library, with builtin support for JSON, MessagePack, YAML, and TOML
- [msgpack](https://github.com/msgpack/msgpack-python): A MessagePack serializer implementation for Python

### Data Processing

#### Character Encoding

- [ftfy](https://github.com/LuminosoInsight/python-ftfy): A library that fixes mojibake and other glitches in Unicode text, after the fact
- [unidecode](https://pypi.python.org/pypi/Unidecode): An ASCII transliterations of Unicode text
- [chardet](https://github.com/chardet/chardet): A Python character encoding detector
- [cchardet](https://github.com/PyYoshi/cChardet): A universal character encoding detector

#### Date and Time

- [datetime](https://docs.python.org/3/library/datetime.html): The Python Standard Library module for manipulating dates and times
- [dateutil](https://github.com/dateutil/dateutil): A library that provides useful extensions to the standard Python datetime features

#### Prices

- [price-parser](https://github.com/scrapinghub/price-parser): A library that extracts price amount and currency symbol from a raw text string

#### Human Names

- [python-nameparser](https://github.com/derek73/python-nameparser): A simple Python module for parsing human names into their individual components

#### Phone Numbers

- [phonenumbers](https://github.com/daviddrysdale/python-phonenumbers): A Python port of Google's [libphonenumber](https://github.com/google/libphonenumber)

#### Slugs

- [python-slugify](https://github.com/un33k/python-slugify): A Python library that returns unicode slugs

#### URLs and Network Addresses

- [netaddr](https://github.com/drkjam/netaddr): A network address manipulation library for Python
- [tldextract](https://github.com/john-kurkowski/tldextract): A library to accurately separates a URL's subdomain, domain, and public suffix, using the Public Suffix List (PSL)

#### Languages

- [xpinyin](https://github.com/lxneng/xpinyin): A library to translate Chinese hanzi to pinyin (拼音) by Python
- [pytils](https://github.com/j2a/pytils): A library that provides Russian-specific string utils

### Other

#### Multiprocessing

- [threading](http://docs.python.org/3/library/threading.html): A Python Standard Library module for thread-based parallelism
- [multiprocessing](http://docs.python.org/3/library/multiprocessing.html): A Python Standard Library module for Process-based parallelism
- [concurrent-futures](https://docs.python.org/3/library/concurrent.futures.html): A Python Standard Library module that provides a high-level interface for asynchronously executing callables

#### Task Scheduling
- [apscheduler](https://github.com/agronholm/apscheduler): A task scheduling library for Python
- [python-crontab](https://gitlab.com/doctormo/python-crontab): A crontab module for reading and writing crontab files and accessing the system cron automatically and simply using a direct API

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: requests, HTTPX, AIOHTTP, or urllib3
- **HTML Parser**: Beautiful Soup or lxml

#### All-In-One Web Scraping Framework

- Scrapy or requests-html

### Dynamic Web Pages

#### All-In-One Browser Automation Framework

- Selenium, Playwright, or pyppeteer

#### Web Scraping Framework + JavaScript Engine

- **Web Scraping Framework**: Scrapy
- **JavaScript Engine**: scrapy-splash

## Guides and Tutorials

### General Guides

- [Web Scraping With Python – 2024 Full Guide](https://brightdata.com/blog/how-tos/web-scraping-with-python)
- [Scraping Dynamic Websites with Python - 2024 Guide](https://brightdata.com/blog/how-tos/scrape-dynamic-websites-python)
- [Web Crawling with Python - 2024 Guide](https://brightdata.com/blog/how-tos/web-crawling-with-python)
- [Master Python HTTP Requests: Advanced Guide 2024](https://brightdata.com/blog/web-data/python-requests-guide)
- [BeautifulSoup Web Scraping: Step-By-Step Tutorial](https://brightdata.com/blog/how-tos/beautiful-soup-web-scraping)
- [Guide to Web Scraping With Selenium in 2024](https://brightdata.com/blog/how-tos/using-selenium-for-web-scraping)
- [How to Use lxml for Web Scraping](https://brightdata.com/blog/web-data/lxml-web-scraping)
- [Using cURL with Python Guide](https://brightdata.com/blog/how-tos/curl-with-python)
- [Downloading Web Pages With Python and Wget](https://brightdata.com/blog/how-tos/wget-with-python)
- [Scraping Images From a Website in Python - 2024 Guide](https://brightdata.com/blog/how-tos/scrape-images-from-websites)

### Proxies

- [Python Proxy Server - What is it?](https://brightdata.com/blog/proxy-101/python-proxy-server)
- [Guide to Using a Proxy with Python Requests](https://brightdata.com/blog/proxy-101/proxy-with-python-requests)
- [How to Set Proxy in AIOHTTP](https://brightdata.com/blog/how-tos/proxy-in-aiohttp)

### User Agent Setting

- [Python Requests User Agent Guide: Setting and Changing](https://brightdata.com/blog/web-data/requests-user-agent)

### Parsing

- [The Best 5 Python HTML Parsers](https://brightdata.com/blog/web-data/best-python-html-parsers)
- [The Best Python HTTP Clients for Web Scraping](https://brightdata.com/blog/web-data/best-python-http-clients)
- [How to Parse JSON in Python](https://brightdata.com/blog/how-tos/parse-json-data-with-python)
- [How to Parse XML in Python? Multiple Methods Covered](https://brightdata.com/blog/how-tos/parsing-xml-in-python)

### Scraping Popular Sites

- [Ultimate Guide to Scraping Google Search With Python](https://brightdata.com/blog/web-data/scraping-google-with-python)
- [How to Scrape YouTube with Python Guide](https://brightdata.com/blog/how-tos/how-to-scrape-youtube-in-python)
- [How to Scrape LinkedIn: 2024 Guide](https://brightdata.com/blog/how-tos/linkedin-scraping-guide)
- [How to Scrape Airbnb: 2024 Guide](https://brightdata.com/blog/how-tos/how-to-scrape-airbnb-guide)
- [How To Scrape Yelp in Python Guide](https://brightdata.com/blog/how-tos/how-to-scrape-yelp-guide)
- [How to Scrape Yahoo Finance - 2024 Guide](https://brightdata.com/blog/how-tos/scrape-yahoo-finance-guide)
- [How to Scrape Craigslist With Python: Step-By-Step Guide](https://brightdata.com/blog/how-tos/how-to-scrape-craigslist-in-python)
- [How To Scrape GitHub Repositories in Python](https://brightdata.com/blog/how-tos/how-to-scrape-github-repositories-in-python)
- [How to Scrape Amazon: 2024 Guide](https://brightdata.com/blog/how-tos/how-to-scrape-amazon)
- [How To Scrape Reddit in Python Guide](https://brightdata.com/blog/web-data/how-to-scrape-reddit-python)
- [How to Scrape Glassdoor: Step-By-Step Guide 2024](https://brightdata.com/blog/web-data/how-to-scrape-glassdoor)
- [How To Build a Zalando Scraper](https://brightdata.com/blog/how-tos/how-to-build-a-zalando-scraper-with-python)
- [How To Scrape eBay in Python For Price Monitoring](https://brightdata.com/blog/how-tos/how-to-scrape-ebay-in-python)

### Anti-Bot Bypass

- [Bypassing CAPTCHAs with Python: Techniques for 2024](https://brightdata.com/blog/web-data/bypass-captchas-with-python)
- [Guide to Web Scraping With cURL Impersonate](https://brightdata.com/blog/web-data/web-scraping-with-curl-impersonate)
- [How to bypass CAPTCHAs with Selenium in Python](https://brightdata.com/blog/web-data/bypass-captchas-with-selenium)
- [Avoiding Bot Detection with Playwright Stealth](https://brightdata.com/blog/how-tos/avoid-bot-detection-with-playwright-stealth)

### Comparisons

- [JavaScript vs Python for Web Scraping Comparison](https://brightdata.com/blog/web-data/javascript-vs-python)
- [Java vs Python - Comparison Guide](https://brightdata.com/blog/web-data/java-vs-python)
- [C# vs. Python for Web Scraping Guide](https://brightdata.com/blog/how-tos/c-sharp-vs-python-for-web-scraping)
- [Go vs. Python - Comparison Guide](https://brightdata.com/blog/web-data/go-vs-python)
- [Python vs. C++ for Web Scraping](https://brightdata.com/blog/web-data/python-vs-c-plus-plus-for-web-scraping)
- [Scrapy vs. Beautiful Soup: Detailed Comparison](https://brightdata.com/blog/web-data/scrapy-vs-beautiful-soup)
- [Scrapy vs. Selenium: Which One to Choose?](https://brightdata.com/blog/web-data/scrapy-vs-selenium)
- [Scrapy vs Puppeteer for Web Scraping](https://brightdata.com/blog/web-data/scrapy-vs-puppeteer)
