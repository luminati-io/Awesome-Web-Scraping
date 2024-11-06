# Ruby Web Scraping

This document contains a list of gems and resources for web scraping in Ruby.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [HTTP Clients](#http-clients)
    - [WebSockets](#websockets)
    - [Low Level](#low-level)
    - [Other](#other)
  - [Parsers](#parsers)
    - [HTML and XML Parsers](#html-and-xml-parsers)
    - [Date and Time Parsers](#date-and-time-parsers)
    - [PDF Parsers](#pdf-parsers)
    - [HTTP Parsers](#http-parsers)
    - [URL Parsers](#url-parsers)
    - [Email Parsers](#email-parsers)
    - [Markdown Parsers](#markdown-parsers)
    - [SQL Parsers](#sql-parsers)
    - [Office File Parsers](#office-file-parsers)
    - [Other](#other-1)
  - [Web Scraping](#web-scraping)
    - [Frameworks](#frameworks)
    - [Tools and Plugins](#tools-and-plugins)
    - [Other](#other-2)
    - [Proxy Integration](#proxy-integration)
    - [CAPTCHA Solving](#captcha-solving)
  - [Web Automation](#web-automation)
    - [Browser Automation Frameworks](#browser-automation-frameworks)
  - [Data Export](#data-export)
    - [JSON](#json)
    - [CSV](#csv)
    - [Other](#other-3)
  - [Data Processing](#data-processing)
    - [General](#general)
    - [Character Encoding](#character-encoding)
    - [Prices](#prices)
    - [Phone Numbers](#phone-numbers)
    - [Units of Measurement](#units-of-measurement)
    - [URLs and Network Addresses](#urls-and-network-addresses)
    - [Languages](#languages)
  - [Other](#other-4)
    - [Multiprocessing](#multiprocessing)
    - [Even Handling](#even-handling)
    - [Task Scheduling](#task-scheduling)
- [Popular Web Scraping Stacks](#popular-web-scraping-stacks)
  - [Static Web Pages](#static-web-pages)
    - [HTTP Client + HTML Parser](#http-client-html-parser)
    - [All-In-One Solution](#all-in-one-solution)
  - [Dynamic Web Pages](#dynamic-web-pages)
- [Guides and Tutorials](#guides-and-tutorials)
  - [General Guides](#general-guides)
  - [Comparisons](#comparisons)

## Libraries

**Note**: All selected gems are either widely used or actively maintained and compatible with Ruby 3+.

### Network

#### HTTP Clients

- [httparty](https://github.com/jnunemaker/httparty): Makes http fun again!
- [HTTP](https://github.com/httprb/http.rb): A fast Ruby HTTP client with a chainable API, streaming support, and timeouts
- [Typhoeus](https://github.com/typhoeus/typhoeus): A gem that wraps [libcurl](https://curl.se/libcurl/) in order to make fast and reliable requests
- [excon](https://github.com/excon/excon): Usable, fast, simple HTTP 1.1 for Ruby
- [nestful](https://github.com/maccman/nestful): A simple Ruby HTTP/REST client with a sane API
- [Faraday](https://github.com/lostisland/faraday): A simple, but flexible HTTP client library, with support for multiple backends
- [EM-HTTP-Request](https://github.com/igrigorik/em-http-request): An asynchronous HTTP Client (EventMachine + Ruby)
- [Http Client](https://github.com/nahi/httpclient): A gem that gives something like the functionality of libwww-perl (LWP) in Ruby
- [Http-2](https://github.com/igrigorik/http-2): A pure Ruby implementation of HTTP/2 protocol
- [Patron](https://github.com/toland/patron): A Ruby HTTP client based on libcurl
- [REST Client](https://github.com/rest-client/rest-client): A simple HTTP and REST client for Ruby, inspired by microframework syntax for specifying actions
- [Spyke](https://github.com/balvig/spyke): A gem to interact with REST services in an ActiveRecord-like manner

#### WebSockets

- [WebSocket Ruby](https://github.com/imanel/websocket-ruby): A universal Ruby library to handle WebSocket protocol
- [faye-websocket](https://github.com/faye/faye-websocket-ruby): A standards-compliant WebSocket client and server

#### Low Level

- [PacketFu](https://github.com/packetfu/packetfu): A mid-level packet manipulation library for Ruby
- [PacketGen](https://github.com/lemontree55/packetgen): A Ruby library to easily generate and capture network packets

#### Other

- [Sawyer](https://github.com/lostisland/sawyer): An experimental hypermedia agent for Ruby built on top of Faraday

### Parsers

#### HTML and XML Parsers

- [Nokogiri](https://github.com/sparklemotion/nokogiri): A gem that makes it easy and painless to work with XML and HTML from Ruby
- [Oga](https://github.com/YorickPeterse/oga): An XML/HTML parser written in Ruby
- [Ox](https://github.com/ohler55/ox): A Ruby optimized XML parser
- [equivalent-xml](https://github.com/mbklein/equivalent-xml) - Easy tests of equivalency of XML documents for Nokogiri::XML

#### Date and Time Parsers

- [date_validator](https://github.com/codegram/date_validator): A simple, ORM agnostic, Ruby >=2.2 compatible date validator for Rails, based on ActiveModel
- [Chronic](https://github.com/mojombo/chronic): A pure Ruby natural language date parser

#### PDF Parsers

- [PDF::Reader](https://github.com/yob/pdf-reader): A library that implements a PDF parser conforming as much as possible to the PDF specification from Adobe

#### HTTP Parsers

- [http_parser.rb](https://github.com/tmm1/http_parser.rb): A simple callback-based HTTP request/response parser

#### URL Parsers

- [Addressable](https://github.com/sporkmonger/addressable): An alternative implementation to the URI implementation that is part of Ruby's standard library. It is flexible, offers heuristic parsing, and additionally provides extensive support for IRIs and URI templates

#### Email Parsers

- [Mail](https://github.com/mikel/mail): A internet library for Ruby that is designed to handle email generation, parsing and sending in a simple, rubyesque manner

#### Markdown Parsers

- [Redcarpet](): A Ruby library for Markdown processing that smells like butterflies and popcorn

#### SQL Parsers

- [pg_query](https://github.com/pganalyze/pg_query): A Ruby extension to parse, deparse and normalize SQL queries using the PostgreSQL query parser

#### Office File Parsers

- [Xsv](https://github.com/martijn/xsv): A high performance, lightweight .xlsx parser for Ruby that provides nothing a CSV parser wouldn't

#### Other

- [loofah](https://github.com/flavorjones/loofah): A Ruby library for HTML/XML transformation and sanitization
- [HappyMapper](https://github.com/dam5s/happymapper): An Object to XML mapping library, using Nokogiri
- [Ruby CSS Parser](https://github.com/premailer/css_parser): A Ruby CSS parser
- [Ruby Readability](https://github.com/cantino/ruby-readability): A Ruby gem to break apart documents into images, text, pages, and PDFs
- [ROXML](https://github.com/Empact/roxml): A module for binding Ruby classes to XML
- [Sitemap Parser](https://github.com/benbalter/sitemap-parser): A gem to parse Sitemaps.org compliant sitemaps
- [RSS](https://github.com/ruby/rss): RSS reading and writing

### Web Scraping

#### Frameworks

- [Mechanize](https://github.com/sparklemotion/mechanize): A ruby library that makes automated web interaction easy
- [Wombat](https://github.com/felipecsl/wombat): A lightweight Ruby web crawler/scraper with an elegant DSL which extracts structured data from pages
- [Spidr](https://github.com/postmodern/spidr): A versatile Ruby web spidering library that can spider a site, multiple domains, certain links or infinitely. Spidr is designed to be fast and easy to use
- [Metainspector](https://github.com/jaimeiniesta/metainspector): A Ruby gem for web scraping purposes. It scrapes a given URL, and returns you its title, meta description, meta keywords, links, images, etc
- [Upton](https://github.com/propublica/upton): A batteries-included framework for easy web-scraping

#### Tools and Plugins

- [HTML::Pipeline](https://github.com/jch/html-pipeline): A library that provides HTML processing filters and utilities

#### Other

- [docsplit](http://documentcloud.github.io/docsplit/): A command-line utility and Ruby library for splitting apart documents into their component parts

#### Proxy Integration

- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]

#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]
- [Ruby 2Captcha API Client](https://github.com/2captcha/2captcha-ruby): A Ruby gem for easy integration with the API of 2Captcha captcha solving service to bypass reCAPTCHA, hCaptcha, FunCaptcha, geetest and solve any other CAPTCHAs

### Web Automation

#### Browser Automation Frameworks

- [selenium-webdriver](https://github.com/SeleniumHQ/selenium/wiki/Ruby-Bindings): The Ruby bindings for [Selenium/WebDriver](https://www.selenium.dev/)
- [Watir](https://github.com/watir/watir): A Ruby gem that facilitates the writing of automated tests by mimicing the behavior of a user interacting with a website
- [playwright-ruby-client](https://github.com/YusukeIwaki/playwright-ruby-client): A [Playwright](https://playwright.dev/) client for Ruby
- [puppeteer-ruby](https://github.com/YusukeIwaki/puppeteer-ruby): A Ruby port of [Puppeteer](https://pptr.dev/)

### Data Export

#### JSON

- [JSON:API](https://github.com/jsonapi-serializer/jsonapi-serializer): A fast JSON:API serializer for Ruby
- [Panko](https://github.com/yosiat/panko_serializer): A high Performance JSON Serialization for ActiveRecord & Ruby Objects
- [JSON](https://ruby-doc.org/3.3.5/exts/json/JSON.html): A built-in Ruby library for dealing with JSON data
- [oj](https://github.com/ohler55/oj): A fast JSON parser and Object marshaller as a Ruby gem

#### CSV

- [CSV](https://ruby-doc.org/3.3.5/stdlibs/csv/CSV.html): A built-in Ruby gem for dealing with CSV files and data
- [SmarterCSV](https://github.com/tilo/smarter_csv): A Ruby gem for convenient reading and writing of CSV files

#### Other

- [HexaPDF](https://github.com/gettalong/hexapdf): A versatile PDF creation and manipulation library for Ruby
- [YAML](https://ruby-doc.org/3.3.5/stdlibs/yaml/YAML.html): A built-in Ruby interface for data serialization in YAML format
- [docx](https://github.com/ruby-docx/docx): A ruby library/gem for interacting with .docx files

### Data Processing

#### General

- [Kiba](https://github.com/thbar/kiba): Data processing & ETL framework for Ruby

#### Character Encoding

- [Encoding::Converter](https://ruby-doc.org/3.3.5/Encoding/Converter.html): A built-in Ruby encoding conversion class

#### Prices

- [RubyMoney](https://github.com/RubyMoney/money): A Ruby Library for dealing with money and currency conversion

#### Phone Numbers

- [Phonelib](https://github.com/daddyz/phonelib): A Ruby gem for phone validation and formatting using google libphonenumber library data
- [phone](https://github.com/carr/phone): A Ruby library for phone number parsing, validation and formatting

#### Units of Measurement

- [Ruby Units](https://github.com/olbrich/ruby-units): A unit handling library for Ruby
- [Unitwise](https://github.com/joshwlewis/unitwise): Physical quantity and units of measure conversion and math for Ruby

#### URLs and Network Addresses

- [Bundler::URI](https://ruby-doc.org/3.3.5/stdlibs/bundler/Bundler/URI.html): A built-in Ruby module providing classes to handle Uniform Resource Identifiers (RFC2396)

#### Languages

- [ChinesePinyin](https://github.com/flyerhzm/chinese_pinyin): A Ruby gem to translate chinese Hanzi to Pinyin

### Other

#### Multiprocessing

- [Thread](https://ruby-doc.org/3.3.5/Thread.html): A built-in Ruby implementation for a concurrent programming model
- [Concurrent Ruby](https://github.com/ruby-concurrency/concurrent-ruby): Modern concurrency tools including agents, futures, promises, thread pools, supervisors, and more. Inspired by Erlang, Clojure, Scala, Go, Java, JavaScript, and classic concurrency patterns
- [Celluloid](https://github.com/celluloid/celluloid): An actor-based concurrent object framework for Ruby
- [Parallel](https://github.com/grosser/parallel):A Ruby gem that makes parallel processing simpler and faster
- [childprocess](https://github.com/jarib/childprocess): A cross-platform Ruby library for managing child processes

#### Even Handling

- [EventMachine](https://github.com/eventmachine/eventmachine): A fast, simple event-processing library for Ruby programs

#### Task Scheduling

- [rufus-scheduler](https://github.com/jmettraux/rufus-scheduler): A scheduler for Ruby (at, in, cron and every jobs)

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: httparty

- **HTML Parser**: Nokogiri

#### All-In-One Solution

- Mechanize

### Dynamic Web Pages

- selenium-webdriver, Watir, or playwright-ruby-client

## Guides and Tutorials

### General Guides

- [Web Scraping with Ruby: Complete Guide {2024 Updated}](https://brightdata.com/blog/how-tos/web-scraping-with-ruby)

### Comparisons

- [Ruby vs JavaScript: Which Should You Choose?](https://brightdata.com/blog/web-data/ruby-vs-javascript)
- [Playwright vs. Selenium Comparison 2024](https://brightdata.com/blog/web-data/playwright-vs-selenium)
