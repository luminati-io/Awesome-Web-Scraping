# Go Web Scraping

This document contains a list of libraries and resources for web scraping in Go.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [HTTP Clients](#http-clients)
    - [WebSockets](#websockets)
    - [Low Level](#low-level)
    - [Other](#other)
  - [Parsers](#parsers)
    - [HTML/XML Parsers](#html-xml-parsers)
    - [URL Parsers](#url-parsers)
    - [Date and Time Parsers](#date-and-time-parsers)
    - [JSON Parsers](#json-parsers)
    - [PDF Parsers](#pdf-parsers)
    - [Email Parsers](#email-parsers)
    - [Markdown Parsers](#markdown-parsers)
    - [SQL Parsers](#sql-parsers)
    - [Other](#other-1)
  - [Web Scraping](#web-scraping)
    - [Frameworks](#frameworks)
    - [Proxy Integration](#proxy-integration)
    - [CAPTCHA Solving](#captcha-solving)
  - [Web Automation](#web-automation)
    - [Browser Automation Frameworks](#browser-automation-frameworks)
    - [Tools and Plugins](#tools-and-plugins)
    - [Other](#other-2)
  - [Data Export](#data-export)
    - [Serialization](#serialization)
    - [JSON](#json)
    - [CSV](#csv)
    - [Other](#other-3)
  - [Data Processing](#data-processing)
    - [Text](#text)
    - [Character Encoding](#character-encoding)
    - [Date and Time](#date-and-time)
    - [Phone Numbers](#phone-numbers)
    - [Slugs](#slugs)
  - [Other](#other-4)
    - [Multiprocessing](#multiprocessing)
    - [Task Scheduling](#task-scheduling)
- [Popular Web Scraping Stacks](#popular-web-scraping-stacks)
  - [Static Web Pages](#static-web-pages)
    - [HTTP Client + HTML Parser](#http-client---html-parser)
    - [All-In-One Web Scraping Framework](#all-in-one-web-scraping-framework)
  - [Dynamic Web Pages](#dynamic-web-pages)
    - [All-In-One Browser Automation Framework](#all-in-one-browser-automation-framework)
- [Guides and Tutorials](#guides-and-tutorials)
  - [General Guides](#general-guides)
  - [Proxies](#proxies)
  - [Comparisons](#comparisons)

## Libraries

**Note**: All selected libraries are either widely used or actively maintained.

### Network

#### HTTP Clients

- [net/http](https://pkg.go.dev/net/http): A built-in Go package that provides HTTP client and server implementations
- [fasthttp](https://github.com/valyala/fasthttp): A fast HTTP implementation for Go
- [resty](https://github.com/go-resty/resty): A simple HTTP and REST client library for Go
- [req](https://github.com/imroc/req): A simple Go HTTP client with Black Magic
- [requests](https://github.com/earthboundkid/requests): HTTP requests for Gophers
- [heimdall](https://github.com/gojek/heimdall): An enhanced HTTP client for Go
- [go-retryablehttp](https://github.com/hashicorp/go-retryablehttp): A retryable HTTP client in Go
- [retryablehttp-go](https://github.com/projectdiscovery/retryablehttp-go): A package that provides a familiar HTTP client interface with automatic retries and exponential backoff
- [sling](https://github.com/dghubble/sling): A Go HTTP client library for creating and sending API requests
- [gorequest](https://github.com/parnurzeal/gorequest): A simplified HTTP client (inspired by Node.js's [SuperAgent](https://ladjs.github.io/superagent/))

#### WebSockets

- [gorilla](https://github.com/gorilla/websocket): A fast, well-tested and widely used WebSocket implementation for Go
- [websocket](https://github.com/coder/websocket): A minimal and idiomatic WebSocket library for Go

#### Low Level

- [net](https://pkg.go.dev/net): A built-in Go portable interface for network I/O, including TCP/IP, UDP, domain name resolution, and Unix domain sockets
- [gots](https://github.com/Comcast/gots): A Go library for MPEG transport stream handling in Go

#### Other

- [caddy](https://github.com/caddyserver/caddy): A fast and extensible multi-platform HTTP/1-2-3 web server with automatic HTTPS

### Parsers

#### HTML/XML Parsers

- [goquery](https://github.com/PuerkitoBio/goquery): A package that brings a syntax and a set of features similar to [jQuery](https://jquery.com/) to the Go language
- [encoding/xml](https://pkg.go.dev/encoding/xml): A built-in Go simple XML 1.0 parser that understands XML name spaces
- [net/html](https://pkg.go.dev/golang.org/x/net/html): A built-in Go Package html implements an HTML5-compliant tokenizer and parser
- [xml-stream-parser](https://github.com/tamerh/xml-stream-parser): An XML stream parser for GO
- [pagser](https://github.com/foolin/pagser): A simple, extensible, configurable parse and deserialize html page to struct based on goquery and struct tags for golang crawler

#### URL Parsers

- [net/url](https://pkg.go.dev/net/url): A built-in Go package that parses URLs and implements query escaping
- [urlquery](https://github.com/hetiansu5/urlquery): A URL query string encoder and parser based on Go

#### Date and Time Parsers

- [dateparse](https://github.com/araddon/dateparse): A library to parse many date strings without knowing format in advance

#### JSON Parsers

- [jsonparser](https://github.com/buger/jsonparser): One of the fastest alternative JSON parser for Go that does not require schema

#### PDF Parsers

- [pdfcpu](https://github.com/pdfcpu/pdfcpu): A PDF processor written in Go
- [pdf](https://github.com/ledongthuc/pdf): A PDF reader in Golang

#### Email Parsers

- [net/mail](https://pkg.go.dev/net/mail): A built-in Go package that implements parsing of mail messages

#### Markdown Parsers

- [markdown](https://github.com/gomarkdown/markdown): A Markdown parser and HTML renderer for Go
- [blackfriday](https://github.com/russross/blackfriday): A Markdown processor for Go
- [goldmark](https://github.com/yuin/goldmark): A Markdown parser written in Go. Easy to extend, standard ([CommonMark](https://commonmark.org/)) compliant, well structured

#### SQL Parsers

- [vitess-sqlparser](https://github.com/blastrain/vitess-sqlparser): A simple SQL parser for Go (Powered by vitess and TiDB)
- [sqlparser](https://github.com/xwb1989/sqlparser): An SQL Parser implemented in Go

#### Other

- [grobotstxt](https://github.com/jimsmart/grobotstxt): A native Go port of Google's robots.txt parser and matcher library
- [gofeed](https://github.com/mmcdole/gofeed): A library to parse RSS, Atom and JSON feeds in Go
- [go-flags](https://github.com/jessevdk/go-flags): A Go command line option parser
- [toml](https://github.com/BurntSushi/toml): A TOML parser for Golang with reflection

### Web Scraping

#### Frameworks

- [colly](https://github.com/gocolly/colly): An elegant scraper and crawler framework for Golang
- [surf](https://github.com/headzoo/surf): A library for stateful programmatic web browsing in Go
- [gospider](https://github.com/jaeles-project/gospider): A fast web spider written in Go
- [ferret](https://github.com/MontFerret/ferret): A library for declarative web scraping
- [pholcus](https://github.com/andeya/pholcus): A distributed high-concurrency crawler software written in pure golang

#### Proxy Integration

- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]
- [goproxy](https://github.com/elazarl/goproxy): An HTTP proxy library for Go

#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver
  that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]
- [captcha](https://github.com/dchest/captcha): A package that implements generation and verification of image and audio CAPTCHAs

### Web Automation

#### Browser Automation Frameworks

- [chromedp](https://github.com/chromedp/chromedp): A faster, simpler way to drive browsers supporting the [Chrome DevTools Protocol](https://chromedevtools.github.io/devtools-protocol/)
- [rod](https://github.com/go-rod/rod): A Chrome DevTools Protocol driver for web automation and scraping
- [selenium](https://github.com/tebeka/selenium): A Selenium/Webdriver client for Go
- [playwright-go](https://github.com/playwright-community/playwright-go): A browser automation library to control Chromium, Firefox and WebKit with a single API. A port of [Playwright](https://playwright.dev/) for Go

#### Tools and Plugins

- [go-rod/stealth](https://github.com/go-rod/stealth): A plugin for anti-bot-detection with rod

#### Other

- [robotgo](https://pkg.go.dev/github.com/go-vgo/robotgo): A Go native cross-platform RPA and GUI automation library

### Data Export

#### Serialization

- [mus-go](https://github.com/mus-format/mus-go): A set of serialization primitives for Golang

#### JSON

- [encoding/json](https://pkg.go.dev/encoding/json): A built-in Go package that implements encoding and decoding of JSON as defined in RFC 7159.

#### CSV

- [encoding/csv](https://pkg.go.dev/encoding/csv): A built-in Go packate that reads and writes comma-separated values (CSV) files

#### Other

- [unioffice](https://github.com/unidoc/unioffice): A pure go library for creating and processing Office Word (.docx), Excel (.xlsx) and Powerpoint (.pptx) documents
- [yaml](https://github.com/go-yaml/yaml): YAML support for the Go language

### Data Processing

#### Text

- [x/text](https://pkg.go.dev/golang.org/x/text): Built-in Go libraries for text processing, many involving Unicode
- [strings](https://pkg.go.dev/strings): A built-in Go package that implements simple functions to manipulate UTF-8 encoded strings

#### Character Encoding

- [enconding](https://pkg.go.dev/encoding): A built-in Go libary that defines interfaces shared by other packages that convert data to and from byte-level and textual representations
- [utf8](https://pkg.go.dev/unicode/utf8): A built-in Go package that implements functions and constants to support text encoded in UTF-8

#### Date and Time

- [time](https://pkg.go.dev/time): A built-in Go package that provides functionality for measuring and displaying time
- [goment](https://github.com/nleeper/goment): A Go time library inspired by [Moment.js](https://momentjs.com/)
- [now](https://github.com/jinzhu/now): A time toolkit for golang
- [carbon](https://github.com/golang-module/carbon): A simple, semantic and developer-friendly golang package for time

#### Phone Numbers

- [phonenumbers](https://github.com/nyaruka/phonenumbers): The GoLang port of Google's libphonenumber library
- [phonenumber](https://github.com/dongri/phonenumber): A library that, with a given country and phone number, validates and formats the mobile phone number to E.164 standard

#### Slugs

- [slug](https://github.com/gosimple/slug): A URL-friendly slugify with multiple languages support

### Other

#### Multiprocessing

- [async](https://github.com/StudioSol/async): A safe way to execute functions asynchronously, recovering them in case of panic. It also provides an error stack aiming to facilitate fail causes discovery

#### Task Scheduling

- [gocron](https://github.com/jasonlvhit/gocron): A Golang job scheduling package
- [go-quartz](https://github.com/reugn/go-quartz): A minimalist and zero-dependency scheduling library for Go
- [cron](https://github.com/robfig/cron): A cron library for Go

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: net/http, req, or go-retryablehttp
- **HTML Parser**: goquery

#### All-In-One Web Scraping Framework

- colly

### Dynamic Web Pages

#### All-In-One Browser Automation Framework

- chromedp, rod, or playwright-go

## Guides and Tutorials

### General Guides

- [Web Scraping in Go: Complete Guide](https://brightdata.com/blog/how-tos/web-scraping-go)

### Proxies

- [Go Proxy Servers – Set Proxy Servers with Go Guide](https://brightdata.com/blog/how-tos/go-proxy-servers)

### Comparisons

- [Go vs. Python - Comparison Guide](https://brightdata.com/blog/web-data/go-vs-python)