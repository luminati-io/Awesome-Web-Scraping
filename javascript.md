# JavaScript Web Scraping

This document contains a list of libraries and resources for web scraping in JavaScript.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [HTTP Clients](#http-clients)
    - [WebSockets](#websockets)
    - [Low Level](#low-level)
    - [Other](#other)
  - [Parsers](#parsers)
    - [HTML/XML Parsers](#htmlxml-parsers)
    - [URL Parsers](#url-parsers)
    - [CSV Parsers](#csv-parsers)
    - [PDF Parsers](#pdf-parsers)
    - [HTTP Parsers](#http-parsers)
    - [Email Parsers](#email-parsers)
    - [Markdown Parsers](#markdown-parsers)
    - [YAML Parsers](#yaml-parsers)
    - [SQL Parsers](#sql-parsers)
    - [Office File Parsers](#office-file-parsers)
    - [Other](#other-1)
  - [Web Scraping](#web-scraping)
    - [Frameworks](#frameworks)
    - [Anti-Bot Bypass](#anti-bot-bypass)
    - [Proxy Integration](#proxy-integration)
    - [CAPTCHA Solving](#captcha-solving)
    - [User-Agent Spoofing](#user-agent-spoofing)
  - [Web Automation](#web-automation)
    - [Browser Automation Frameworks](#browser-automation-frameworks)
    - [Tools and Plugins](#tools-and-plugins)
    - [Other](#other-2)
  - [Data Export](#data-export)
    - [JSON](#json)
    - [CSV](#csv)
    - [Other](#other-3)
  - [Data Processing](#data-processing)
    - [Character Encoding](#character-encoding)
    - [Date and Time](#date-and-time)
    - [Prices](#prices)
    - [Phone Numbers](#phone-numbers)
    - [Slugs](#slugs)
    - [Languages](#languages)
  - [Other](#other-4)
    - [Task Scheduling](#task-scheduling)
- [Popular Web Scraping Stacks](#popular-web-scraping-stacks)
  - [Static Web Pages](#static-web-pages)
    - [HTTP Client + HTML Parser](#http-client-html-parser)
    - [All-In-One Web Scraping Framework](#all-in-one-web-scraping-framework)
  - [Dynamic Web Pages](#dynamic-web-pages)
- [Guides and Tutorials](#guides-and-tutorials)
  - [General Guides](#general-guides)
  - [Proxies](#proxies)
  - [User Agent Setting](#user-agent-setting)
  - [Anti-Bot Bypass](#anti-bot-bypass-1)
  - [Comparisons](#comparisons)

## Libraries

**Note**: All selected libraries are actively maintained.

### Network

#### HTTP Clients

- [fetch](https://nodejs.org/dist/latest/docs/api/globals.html#fetch): A built-in Node.js browser-compatible implementation of the [`fetch()`](https://developer.mozilla.org/en-US/docs/Web/API/Window/fetch) function
- [axios](https://github.com/axios/axios): A `Promise`-based HTTP client for the browser and Node.js [**[Axios Proxy Integration](https://brightdata.com/blog/how-tos/axios-proxy)**]
- [node-fetch](https://github.com/bitinn/node-fetch): A light-weight module that brings the Fetch API to Node.js [**[node-fetch Proxy Integration](https://brightdata.com/blog/proxy-101/proxy-in-node-fetch)**]
- [undici](https://www.npmjs.com/package/undici): An HTTP/1.1 client, written from scratch for Node.js
- [superagent](https://github.com/visionmedia/superagent): A small progressive client-side HTTP request library, and Node.js module with the same API, supporting many high-level HTTP client features [**[SuperAgent Proxy Integration](https://brightdata.com/blog/how-tos/superagent-proxy)**]
- [urllib](https://github.com/node-modules/urllib): A library to request HTTP(s) URLs in a complex world
- [node-libcurl](https://github.com/JCMais/node-libcurl): [libcurl](https://curl.se/libcurl/) bindings for Node.js
- [got](https://github.com/sindresorhus/got): A human-friendly and powerful HTTP request library for Node.js
- [bent](https://github.com/mikeal/bent): A functional HTTP client for Node.js w/ async/await
- [needle](https://github.com/tomas/needle): A nimble, streamable HTTP client for Node.js. With proxy, iconv, cookie, deflate & multipart support

#### WebSockets

- [ws](https://github.com/websockets/ws): A simple to use, blazing fast and thoroughly tested WebSocket client and server for Node.js
- [WebScoket-Node](https://github.com/theturtle32/WebSocket-Node): A WebSocket implementation for Node.JS (Draft -08 through the final RFC 6455)

#### Low Level

- [node:net](https://nodejs.org/api/net.html): A built-in Node.js module that provides an asynchronous network API for creating stream-based TCP or IPC servers and clients
- [multicast-dns](https://github.com/mafintosh/multicast-dns): A low-level multicast DNS implementation in pure JavaScript
- [node-ip](https://github.com/indutny/node-ip): IP address tools for node.js

#### Other

- [wreck](https://github.com/hapijs/wreck): HTTP client utilities for the [hapi web framework](https://hapi.dev/)
- [proxy-chain](https://github.com/apify/proxy-chain): A Node.js implementation of a proxy server (think Squid) with support for SSL, authentication and upstream proxy chaining

### Parsers

#### HTML/XML Parsers

- [cheerio](https://github.com/cheeriojs/cheerio): A fast, flexible, and elegant library for parsing and manipulating HTML and XML
- [fast-xml-parser](https://github.com/NaturalIntelligence/fast-xml-parser): A library to validate XML, parse XML, and build XML rapidly without C/C++ based libraries and no callback
- [node-html-parser](https://github.com/taoqf/node-html-parser): A very fast HTML parser, generating a simplified DOM, with basic element query support
- [html-dom-parser](https://github.com/remarkablemark/html-dom-parser): An HTML to DOM parser
- [parse5](https://github.com/inikulin/parse5): An HTML parsing/serialization toolset for Node.js. WHATWG HTML Living Standard (aka HTML5)-compliant
- [htmlparser2](https://github.com/fb55/htmlparser2): A fast and forgiving HTML and XML parser
- [sax-js](https://github.com/isaacs/sax-js): A sax style parser for JS

#### URL Parsers

- [node:url](https://nodejs.org/api/url.html): A built-in Node.js module that provides utilities for URL resolution and parsing
- [query-string](https://github.com/sindresorhus/query-string): A library to parse and stringify URL query strings.
- [URI.js](https://github.com/medialize/URI.js/): A Javascript URL mutation library

#### CSV Parsers

- [csv-parse](https://github.com/adaltas/node-csv/tree/master/packages/csv-parse): A parser converting CSV text input into arrays or objects
- [fast-csv](https://github.com/C2FO/fast-csv): A CSV parser and formatter for Node.js

#### PDF Parsers

- [pdf-parse](https://gitlab.com/autokent/pdf-parse): A pure JavaScript cross-platform module to extract texts from PDFs
- [pdf2json](https://github.com/modesty/pdf2json): A library that converts binary PDF to JSON and text, for server-side PDF processing and command-line use

#### HTTP Parsers

- [http-parser-js](https://github.com/creationix/http-parser-js): A pure JS HTTP parser for Node.js

#### Email Parsers

- [email-reply-parser](https://github.com/crisp-oss/email-reply-parser): A Node.js library for parsing plain text email content
- [email-forward-parser](https://github.com/crisp-oss/email-forward-parser): A library that parses forwarded emails and extracts original content
- [node-address-rfc2822](https://github.com/haraka/node-address-rfc2822): A parser for RFC2822 (Header) format email addresses
- [smtp-address-parser](https://github.com/gene-hightower/smtp-address-parser): A library to parse an SMTP (RFC-5321) address

#### Markdown Parsers

- [markdown-it](https://github.com/markdown-it/markdown-it): A Markdown parser, done right. 100% CommonMark support, extensions, syntax plugins & high speed
- [marked](https://github.com/markedjs/marked): A Markdown parser and compiler. Built for speed
- [micromark](https://github.com/micromark/micromark/tree/main): A small, safe, and great commonmark (optionally gfm) compliant Markdown parser

#### YAML Parsers

- [yaml](https://github.com/eemeli/yaml): A YAML parser and stringifier for JavaScript
- [js-yaml](https://github.com/nodeca/js-yaml): A JavaScript YAML parser and dumper. Very fast
- [yaml-eslint-parser](https://github.com/ota-meshi/yaml-eslint-parser): A YAML parser that produces output compatible with ESLint

#### SQL Parsers

- [node-sql-parser](https://github.com/taozhi8833998/node-sql-parser): Parse simple SQL statements into an abstract syntax tree (AST) with the visited tableList and convert it back to SQL
- [js-sql-parser](https://www.npmjs.com/package/js-sql-parser): An SQL parser written with [jison](https://github.com/zaach/jison). Parses SQL into abstract syntax tree (AST) and stringifies back to SQL

#### Office File Parsers

- [xlsx](https://github.com/SheetJS/sheetjs): A spreadsheet data parser and writer
- [exceljs](https://github.com/exceljs/exceljs): A library to read, manipulate, and write spreadsheet data and styles to XLSX and JSON
- [docx](https://github.com/dolanmiu/docx): A library to easily generate and modify .docx files with JS/TS with a nice declarative API. Works for Node.js and on the browser

#### Other

- [robots-parser](https://github.com/samclarke/robots-parser): A Node.js robots.txt parser with support for wildcard (\*) matching
- [sitemapper](https://github.com/seantomburke/sitemapper): A parser for XML Sitemaps to be used with robots.txt and web crawlers
- [ip-address](https://github.com/beaugunderson/ip-address): A library for parsing and manipulating IPv4 and IPv6 addresses in JavaScript
- [feed-extractor](https://github.com/extractus/feed-extractor): Simplest way to read & normalize RSS/ATOM/JSON feed data
- [sanitize-html](https://github.com/apostrophecms/sanitize-html): A library to Clean up user-submitted HTML, preserving whitelisted elements and whitelisted attributes on a per-element basis. Built on htmlparser2 for speed and tolerance
- [parse-css](https://github.com/tabatkins/parse-css): A standards-based CSS parser
- [js-xss](https://github.com/leizongmin/js-xss): A library to sanitize untrusted HTML (to prevent XSS) with a configuration specified by a Whitelist

### Web Scraping

#### Frameworks

- [crawlee](https://github.com/apify/crawlee): A web scraping and browser automation library for Node.js to build reliable crawlers. In JavaScript and TypeScript. Extract data for AI, LLMs, RAG, or GPTs. Download HTML, PDF, JPG, PNG, and other files from websites. Works with Puppeteer, Playwright, Cheerio, JSDOM, and raw HTTP. Both headful and headless mode. With proxy rotation
- [node-crawler](https://github.com/sylvinus/node-crawler): A web crawler/spider for Node.JS + server-side jQuery
- [ayakashi](https://github.com/ayakashi-io/ayakashi): A next generation web scraping framework
- [webster](https://github.com/zhuyingda/webster): A reliable high-level web crawling & scraping framework for Node.js

#### Anti-Bot Bypass

- [node-curl-impersonate](https://www.npmjs.com/package/node-curl-impersonate): A library that allows you to use [curl-impersonate](https://github.com/lwthiker/curl-impersonate) natively
- [cloudflare-scraper](https://github.com/JimmyLaurent/cloudflare-scraper): A package to bypass Cloudflare's protection
- [unblocker](https://github.com/nfriedly/node-unblocker): A web proxy for evading internet censorship, and general-purpose Node.js library for proxying and rewriting remote webpages

#### Proxy Integration
- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports  state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]

#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver
  that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]
- [nopecha-nodejs](https://github.com/NopeCHALLC/nopecha-nodejs): An automated CAPTCHA solver for Node.js
- [2captcha](https://github.com/Furry/2captcha): A wrapper around the 2Captcha API
- [2captcha-javascript](2captcha-javascript): A JavaScript library for easy integration with the API of 2captcha captcha solving service to bypass reCAPTCHA, hCaptcha, funcaptcha, geetest and solve any other CAPTCHAs

#### User-Agent Spoofing

- [user-agents](https://github.com/intoli/user-agents): A JavaScript library for generating random user agents with data that's updated daily

### Web Automation

#### Browser Automation Frameworks

- [puppeteer](https://github.com/GoogleChrome/puppeteer): A JavaScript library which provides a high-level API to control Chrome or Firefox over the [DevTools Protocol](https://chromedevtools.github.io/devtools-protocol/) or [WebDriver BiDi](https://pptr.dev/webdriver-bidi) [**[Puppeteer Proxy Integration](https://brightdata.com/integration/puppeteer)**]
- [playwright](https://github.com/microsoft/playwright): A framework for Web Testing and Automation. It allows testing Chromium, Firefox and WebKit with a single API [**[Playwright Proxy Integration](https://brightdata.com/integration/playwright)**]
- [selenium](https://github.com/SeleniumHQ/selenium): A browser automation framework and ecosystem [**[Selenium Proxy Integration](https://brightdata.com/integration/selenium)**]
- [cypress](https://github.com/cypress-io/cypress): A fast, easy and reliable testing for anything that runs in a browser
- [webdriverio](https://github.com/webdriverio/webdriverio): A next-gen browser and mobile automation test framework for Node.js
- [wendigo](https://github.com/angrykoala/wendigo): A proper monster for front-end automated testing

#### Tools and Plugins

- [puppeteer-extra-plugin-stealth](https://github.com/berstend/puppeteer-extra/tree/master/packages/puppeteer-extra-plugin-stealth): A plugin for puppeteer-extra and playwright-extra to prevent detection
- [puppeteer-extra-plugin-anonymize-ua](https://github.com/berstend/puppeteer-extra/tree/master/packages/puppeteer-extra-plugin-anonymize-ua): A plugin for puppeteer-extra and playwright-extra to anonymize the User-Agent on all pages
- [@extra/proxy-router](https://github.com/berstend/puppeteer-extra/tree/master/packages/plugin-proxy-router): A plugin for playwright-extra and puppeteer-extra to route proxies dynamically
- [puppeteer-extra-plugin-block-resources](https://github.com/berstend/puppeteer-extra/tree/master/packages/puppeteer-extra-plugin-block-resources): A plugin for playwright-extra and puppeteer-extra to block resources (images, media, css, etc.)

#### Other

- [playwright-extra](https://github.com/berstend/puppeteer-extra/tree/39248f1f5deeb21b1e7eb6ae07b8ef73f1231ab9/packages/playwright-extra): A modular plugin framework for playwright to enable cool plugins through a clean interface
- [puppeteer-extra](https://github.com/berstend/puppeteer-extra): A library to teach puppeteer new tricks through plugins

### Data Export

#### JSON

- [JSON](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON): A built-in JavaScript namespace that contains static methods for parsing values from and converting values to JavaScript Object Notation

#### CSV

- [csv-generate](https://github.com/adaltas/node-csv/tree/master/packages/csv-generate): A flexible generator of random CSV strings and JavaScript objects implementing the Node.js [`stream.Readable`](https://nodejs.org/api/stream.html#class-streamreadable) API

#### Other

- [protobuf.js](https://github.com/protobufjs/protobuf.js): Protocol buffers for JavaScript & TypeScript
- [jBinary](https://github.com/jDataView/jBinary): A high-level API for working with binary data

### Data Processing

#### Character Encoding

- [encoding.js](https://github.com/polygonplanet/encoding.js): A librarry to convert and detect character encoding in JavaScript
- [chardet](https://github.com/runk/node-chardet): A character encoding detection tool for Node.js
- [iconv-lite](https://github.com/ashtuchkin/iconv-lite): A library to convert character encodings in pure JavaScript

#### Date and Time

- [dayjs](https://github.com/iamkun/dayjs): A 2kB immutable date-time library alternative to Moment.js with the same modern API
- [date-fns](https://github.com/date-fns/date-fns): A modern JavaScript date utility library
- [luxon](https://github.com/moment/luxon): A library for working with dates and times in JS

#### Prices

- [money.js](https://github.com/openexchangerates/money.js): A tiny (1kb) javascript currency conversion library, for web & Node.js
- [currency.js](https://github.com/scurker/currency.js): A JavaScript library for handling currencies

#### Phone Numbers

- [libphonenumber-js](https://gitlab.com/catamphetamine/libphonenumber-js): A simpler (and smaller) rewrite of Google Android's libphonenumber library in JavaScript
- [phone](https://github.com/aftership/phone): A library to validate and reformat the mobile phone number to the E.164 standard

#### Slugs

- [unique-slug](https://github.com/npm/unique-slug): A library that slugifies even UTF-8 characters
- [unique-slug](https://github.com/npm/unique-slug): A library to generate a unique character string suitible for use in files and URLs

#### Languages

- [remove-accents](https://github.com/tyxla/remove-accents): A library that removes the accents from a string, converting them to their non-accented corresponding characters
- [nodejieba](https://github.com/yanyiwu/nodejieba): A library that provides Chinese word segmentation for Node.js

### Other

#### Task Scheduling
- [node-schedule](https://github.com/node-schedule/node-schedule): A cron-like and not-cron-like job scheduler for Node
- [node-cron](https://github.com/node-cron/node-cron): A simple cron-like job scheduler for Node.js
- [bree](https://github.com/breejs/bree): A Node.js and JavaScript job task scheduler with worker threads, cron, Date, and human syntax
- [cron](https://github.com/kelektiv/node-cron): A robust tool for running jobs (functions or commands) on schedules defined using the cron syntax


## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: Axios, node-fetch, fetch, or SuperAgent
- **HTML Parser**: Cheerio

#### All-In-One Web Scraping Framework

- Crawlee

### Dynamic Web Pages

- Playwright, Puppeteer, Selenium, or Cypress

## Guides and Tutorials

### General Guides

- [Web Scraping With JavaScript and Node.js Guide](https://brightdata.com/blog/how-tos/web-scraping-with-node-js)
- [Web Scraping With Next.JS in 2024](https://brightdata.com/blog/how-tos/web-scraping-with-next-js)
- [Web Scraping with Crawlee: Step-By-Step Tutorial](https://brightdata.com/blog/web-data/web-scraping-with-crawlee)
- [Using Cheerio NPM for Web Scraping](https://brightdata.com/blog/how-tos/cheerio-npm-web-scraping)
- [Playwright Web Scraping - 2024 Guide](https://brightdata.com/blog/how-tos/playwright-web-scraping)
- [Web Scraping with Puppeteer - 2024 Guide](https://brightdata.com/blog/how-tos/web-scraping-puppeteer)
- [HTTP Requests in Node.js with Fetch API](https://brightdata.com/blog/how-tos/fetch-api-nodejs)

### Proxies

- [How To Set a Proxy in Axios: Definitive Guide](https://brightdata.com/blog/how-tos/axios-proxy)
- [How To Set a Proxy in SuperAgent](https://brightdata.com/blog/how-tos/superagent-proxy)
- [How to Use Proxy in Node-Fetch Guide](https://brightdata.com/blog/proxy-101/proxy-in-node-fetch)
- [How to Use Proxy Servers in Node.js](https://brightdata.com/blog/how-tos/nodejs-proxy-servers)

### User Agent Setting

- [Puppeteer User Agent Guide: Setting and Changing](https://brightdata.com/blog/web-data/puppeteer-user-agent)
- [Node.js User Agent Guide: Setting and Changing](https://brightdata.com/blog/web-data/node-js-user-agent)

### Anti-Bot Bypass

- [Avoiding Bot Detection with Playwright Stealth](https://brightdata.com/blog/how-tos/avoid-bot-detection-with-playwright-stealth)
- [Avoid Getting Blocked With Puppeteer Stealth](https://brightdata.com/blog/how-tos/avoid-getting-blocked-with-puppeteer-stealth)
- [How to Bypass CAPTCHAs with Playwright](https://brightdata.com/blog/web-data/bypass-captchas-with-playwright)
- [Using Node Unblocker for Web Scraping](https://brightdata.com/blog/how-tos/node-unblocker-web-scraping)

### Comparisons

- [JavaScript vs Python for Web Scraping Comparison](https://brightdata.com/blog/web-data/javascript-vs-python)
- [C# vs JavaScript for Web Scraping](https://brightdata.com/blog/web-data/c-sharp-vs-javascript)
- [JavaScript vs Rust for Web Scraping](https://brightdata.com/blog/web-data/javascript-vs-rust-web-scraping)
- [Cheerio vs. Puppeteer for Web Scraping](https://brightdata.com/blog/web-data/cheerio-vs-puppeteer)
- [Puppeteer vs. Selenium - Which One to Choose?](https://brightdata.com/blog/proxy-101/puppeteer-vs-selenium)
- [Scrapy vs Puppeteer for Web Scraping](https://brightdata.com/blog/web-data/scrapy-vs-puppeteer)
- [Playwright vs. Selenium Comparison 2024](https://brightdata.com/blog/web-data/playwright-vs-selenium)
- [Puppeteer vs Playwright for Web Scraping](https://brightdata.com/blog/web-data/puppeteer-vs-playwright)
