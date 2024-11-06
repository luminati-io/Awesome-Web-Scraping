# Rust Web Scraping

This document contains a list of crates and resources for web scraping in Rust.

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
    - [HTTP Parsers](#http-parsers)
    - [CSV Parsers](#csv-parsers)
    - [PDF Parsers](#pdf-parsers)
    - [Email Parsers](#email-parsers)
    - [Markdown Parsers](#markdown-parsers)
    - [YAML Parsers](#yaml-parsers)
    - [SQL Parsers](#sql-parsers)
    - [Office File Parsers](#office-file-parsers)
    - [Other](#other-1)
  - [Web Scraping](#web-scraping)
    - [Frameworks](#frameworks)
    - [Proxy Integration](#proxy-integration)
    - [CAPTCHA Solving](#captcha-solving)
  - [Web Automation](#web-automation)
    - [Browser Automation Frameworks](#browser-automation-frameworks)
    - [Tools and Plugins](#tools-and-plugins)
  - [Data Processing](#data-processing)
  - [Serialization](#serialization)
    - [Character Encoding](#character-encoding)
    - [Text](#text)
    - [Date and Time](#date-and-time)
    - [Phone Numbers](#phone-numbers)
    - [Human Names](#human-names)
    - [Slugs](#slugs)
  - [Other](#other-2)
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

**Note**: All selected crates are either widely used or actively maintained.

### Network

#### HTTP Clients

- [reqwest](https://github.com/seanmonstar/reqwest): An ergonomic, batteries-included HTTP Client for Rust
- [ureq](https://github.com/algesten/ureq): A simple, safe HTTP client
- [curl-rust](https://github.com/alexcrichton/curl-rust): Rust bindings to [libcurl](https://curl.se/libcurl/)
- [attohttpc](https://github.com/sbstp/attohttpc): A Rust lightweight HTTP 1.1 client
- [actix-web](https://github.com/actix/actix-web): A powerful, pragmatic, and extremely fast web framework for Rust
- [isahc](https://github.com/sagebind/isahc): A practical HTTP client that is fun to use

#### WebSockets

- [rust-websocket](https://github.com/websockets-rs/rust-websocket): A WebSocket (RFC6455) library written in Rust
- [tungstenite-rs](https://github.com/snapview/tungstenite-rs): A lightweight stream-based WebSocket implementation for Rust
- [websocket.rs](https://github.com/nurmohammed840/websocket.rs): A WebSocket implementation for both client and server

#### Low Level

- [hyper](https://github.com/hyperium/hyper): A low level protective and efficient HTTP library for all, meant to be a building block for libraries and applications
- [tiny-http](https://github.com/tiny-http/tiny-http): A low-level HTTP server library in Rust
- [libpnet](https://github.com/libpnet/libpnet): A crate for cross-platform, low level networking using the Rust programming language
- [pcap](https://github.com/rust-pcap/pcap): A Rust language crate for accessing the packet sniffing capabilities of libpcap
- [rustls](https://github.com/rustls/rustls): A modern TLS library in Rust

#### Other

- [hyper-util](https://github.com/hyperium/hyper-util): A collection of utilities to do common things with hyper
- [reqwest-middleware](https://github.com/TrueLayer/reqwest-middleware): A Wrapper around reqwest to allow for client middleware chains

### Parsers

#### HTML/XML Parsers

- [scraper](https://github.com/rust-scraper/scraper): HTML parsing and querying with CSS selectors
- [html5ever](https://github.com/servo/html5ever): A high-performance browser-grade HTML5 parser
- [select.rs](https://github.com/utkarshkukreti/select.rs): A Rust library to extract useful data from HTML documents, suitable for web scraping
- [quick-xml](https://github.com/tafia/quick-xml): A Rust high performance XML reader and writer
- [roxmltree](roxmltree): A crate to represent an XML document as a read-only tree

#### URL Parsers

- [rust-url](https://github.com/servo/rust-url): A URL parser for Rust

#### HTTP Parsers

- [https://github.com/seanmonstar/httparse](httparse): A push parser for the HTTP 1.x protocol in Rust

#### CSV Parsers

- [rust-csv](https://github.com/BurntSushi/rust-csv): A CSV parser for Rust, with [Serde](https://serde.rs/) support

#### PDF Parsers

- [pdf-extract](https://github.com/jrmuizel/pdf-extract): A Rust library for extracting content from PDFs

#### Email Parsers

- [mailparse](https://github.com/staktrace/mailparse): A Rust library to parse mail files

#### Markdown Parsers

- [pulldown-cmark](https://github.com/pulldown-cmark/pulldown-cmark): An efficient, reliable parser for [CommonMark](https://commonmark.org/), a standard dialect of Markdown
- [markdown-rs](https://github.com/wooorm/markdown-rs): A CommonMark compliant markdown parser in Rust with ASTs and extensions

#### YAML Parsers

- [yaml-rust](https://github.com/chyh1990/yaml-rust): A pure rust YAML implementation

#### SQL Parsers

- [datafusion-sqlparser-rs](https://github.com/apache/datafusion-sqlparser-rs): An extensible SQL lexer and parser for Rust

#### Office File Parsers

- [calamine](https://github.com/tafia/calamine): A pure Rust Excel/OpenDocument SpreadSheets file reader

#### Other

- [pest](https://github.com/pest-parser/pest): A general purpose parser written in Rust with a focus on accessibility, correctness, and performance
- [rust-cssparser](https://github.com/servo/rust-cssparser): A Rust implementation of CSS Syntax Level 3
- [ammonia](https://github.com/rust-ammonia/ammonia): A crate to repair and secure untrusted HTML
- [ttf-parser](https://github.com/RazrFalcon/ttf-parser): A high-level, safe, zero-allocation TrueType font parser
- [robotstxt](https://github.com/Folyd/robotstxt): A native Rust port of Google's robots.txt parser and matcher C++ library
- [rss](https://github.com/rust-syndication/rss): A library for serializing the RSS web content syndication format
- [collie](https://github.com/collie-reader/collie): A minimal feed reader just for you

### Web Scraping

#### Frameworks

- [spider](https://github.com/spider-rs/spider): A web crawler and scraper for Rust
- [dyer](https://github.com/hominee/dyer): A Rust crate designed for reliable, flexible and fast web crawling, providing some high-level, comprehensive features without compromising speed

#### Proxy Integration

- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]

#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]
- [challenge-bypass-ristretto](https://github.com/brave-intl/challenge-bypass-ristretto): A Rust implemention of the privacy pass cryptographic protocol using the [Ristretto group](https://ristretto.group/)

### Web Automation

#### Browser Automation Frameworks

- [rust-headless-chrome](https://github.com/rust-headless-chrome/rust-headless-chrome): A high-level API to control headless Chrome or Chromium over the DevTools Protocol. It is the Rust equivalent of [Puppeteer](https://pptr.dev/), a Node library maintained by the Chrome DevTools team
- [thirtyfour](https://github.com/Vrtgs/thirtyfour): A Selenium WebDriver client for Rust, for automated testing of websites
- [chromiumoxide](https://github.com/mattsse/chromiumoxide): A Rust crate that provides a high-level and async API to control Chrome or Chromium over the [DevTools Protocol](https://chromedevtools.github.io/devtools-protocol/)
- [playwright-rust](https://github.com/octaltree/playwright-rust): A [Playwright](https://playwright.dev/) port to Rust

#### Tools and Plugins

- [webdriver-downloader](https://github.com/ik1ne/webdriver-downloader): A CLI interface & library for WebDriver download

### Data Processing

### Serialization

- [serde](https://github.com/serde-rs/serde): A serialization framework for Rust

#### Character Encoding

- [rust-base64](https://github.com/marshallpierce/rust-base64): A Rust crate that encodes and decodes base64 as bytes or utf8
- [encoding_rs](https://github.com/hsivonen/encoding_rs): A Gecko-oriented implementation of the [Encoding Standard](https://encoding.spec.whatwg.org/) in Rust

#### Text

- [rust-lexical](https://github.com/Alexhuszagh/rust-lexical): A Rust crate that provides fast numeric to- and from-string conversion routines

#### Date and Time

- [chrono](https://github.com/chronotope/chrono): A date and time library for Rust
- [time](https://github.com/time-rs/time): The most used Rust library for date and time handling
- [httpdate](https://github.com/pyfisch/httpdate): HTTP date parsing and formatting

#### Phone Numbers

- [rust-phonenumber](https://github.com/whisperfish/rust-phonenumber): A library for parsing, formatting and validating international phone numbers

#### Human Names

- [human-name](https://github.com/djudd/human-name): A Rust library for parsing and comparing human names

#### Slugs

- [slug-rs](https://github.com/Stebalien/slug-rs): A small library for generating ASCII slugs from unicode strings

### Other

#### Multiprocessing

- [tokio](https://github.com/tokio-rs/tokio): A runtime for writing reliable asynchronous applications with Rust. Provides I/O, networking, scheduling, timers, etc.
- [rayon](https://github.com/rayon-rs/rayon): A data parallelism library for Rust
- [async-task](https://github.com/smol-rs/async-task): A task abstraction for building executors

#### Task Scheduling

- [clokwerk](https://github.com/mdsherry/clokwerk): A simple scheduler for Rust

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: reqwest, ureq, curl-rust
- **HTML Parser**: scraper, html5ever, select.rs, or quick-xml

#### All-In-One Web Scraping Framework

- spider

### Dynamic Web Pages

#### All-In-One Browser Automation Framework

- rust-headless-chrome, thirtyfour, or chromiumoxide

## Guides and Tutorials

### General Guides

- [Web Scraping With Rust](https://brightdata.com/blog/how-tos/web-scraping-with-rust)

### Proxies

- [Rust Proxy Servers: How to Set Proxy in Rust](https://brightdata.com/blog/how-tos/rust-proxy-servers)

### Comparisons

- [JavaScript vs Rust for Web Scraping](https://brightdata.com/blog/web-data/javascript-vs-rust-web-scraping)
