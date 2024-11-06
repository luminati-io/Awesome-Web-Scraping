# PHP Web Scraping

This document contains a list of libraries and resources for web scraping in PHP.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [HTTP Clients](#http-clients)
    - [WebSockets](#websockets)
  - [Parsers](#parsers)
    - [HTML and XML Parsers](#html-and-xml-parsers)
    - [CSV Parsers](#csv-parsers)
    - [JSON Parsers](#json-parsers)
    - [PDF Parsers](#pdf-parsers)
    - [Email Parsers](#email-parsers)
    - [Markdown Parsers](#markdown-parsers)
    - [YAML Parsers](#yaml-parsers)
    - [SQL Parsers](#sql-parsers)
    - [Office File Parsers](#office-file-parsers)
    - [Other](#other)
  - [Web Scraping](#web-scraping)
    - [Frameworks](#frameworks)
    - [Proxy Integration](#proxy-integration)
    - [CAPTCHA Solving](#captcha-solving)
  - [Web Automation](#web-automation)
    - [Browser Automation Frameworks](#browser-automation-frameworks)
  - [Data Export](#data-export)
    - [JSON](#json)
    - [CSV](#csv)
    - [Other](#other-1)
  - [Data Processing](#data-processing)
    - [General](#general)
    - [Character Encoding](#character-encoding)
    - [Date and Time](#date-and-time)
    - [Prices](#prices)
    - [Phone Numbers](#phone-numbers)
    - [Units of Measurement](#units-of-measurement)
    - [Slugs](#slugs)
    - [URLs and Network Addresses](#urls-and-network-addresses)
  - [Other](#other-2)
    - [Multiprocessing](#multiprocessing)
    - [Even Handling](#even-handling)
    - [Software Automation Management](#software-automation-management)
    - [Task Scheduling](#task-scheduling)
- [Popular Web Scraping Stacks](#popular-web-scraping-stacks)
  - [Static Web Pages](#static-web-pages)
    - [HTTP Client + HTML Parser](#http-client-html-parser)
    - [All-In-One Solution](#all-in-one-solution)
  - [Dynamic Web Pages](#dynamic-web-pages)
- [Guides and Tutorials](#guides-and-tutorials)
  - [General Guides](#general-guides)
  - [Proxies](#proxies)
  - [HTTP Clients](#http-clients-1)

## Libraries

**Note**: All selected libraries are either actively maintained or widely used.

### Network

#### HTTP Clients

- [PHP cURL](https://www.php.net/manual/en/book.curl.php): A built-in PHP library based on [libcurl](https://curl.se/libcurl/) to connect and communicate to many different types of servers with many different types of protocols
- [Guzzle](https://github.com/guzzle/guzzle): A PHP HTTP client that makes it easy to send HTTP requests and trivial to integrate with web services [**[Guzzle proxy integration](https://brightdata.com/blog/how-tos/proxy-with-guzzle)**]
- [HttpClient](https://github.com/symfony/http-client): A Symfony component implementing a low-level HTTP client
- [Buzz](https://github.com/kriswallsmith/Buzz): A lightweight (<1000 lines of code) PHP 7.1 library for issuing HTTP requests
- [amphp/http-client](https://github.com/amphp/http-client): An advanced async HTTP client library for PHP, enabling efficient, non-blocking, and concurrent requests and responses
- [Requests](https://github.com/rmccue/Requests): A humble HTTP request library. It simplifies how you interact with other sites and takes away all your worries.
- [HTTPFul](https://github.com/nategood/httpful): A Chainable, REST-friendly, PHP HTTP client. A sane alternative to cURL.
  with support for both PHP stream wrappers and cURL

#### WebSockets

- [Sockets](https://www.php.net/manual/en/intro.sockets.php): A built-in PHP extension that implements a low-level interface to the socket communication functions based on the popular BSD sockets, providing the possibility to act as a socket server as well as a client
- [Ratchet](https://github.com/ratchetphp/Ratchet): A PHP library for asynchronously serving WebSockets
- [Pawl](https://github.com/ratchetphp/Pawl): An asynchronous WebSocket client in PHP

### Parsers

#### HTML and XML Parsers

- [Simple Html Dom Parser for PHP](https://github.com/voku/simple_html_dom): A modern simple HTML DOM parser for PHP
- [HTML5-PHP](https://github.com/Masterminds/html5-php): An HTML5 parser and serializer for PHP
- [DiDOM](https://github.com/Imangazaliev/DiDOM): A simple and fast HTML and XML parser
- [QueryPath](https://github.com/GravityPDF/querypath) : A PHP library for HTML(5)/XML querying (CSS 4 or XPath) and processing (like jQuery) with PHP8.3 support
- [DomCrawler](https://github.com/symfony/dom-crawler): A Symfony component that eases DOM navigation for HTML and XML documents
- [PHP Html Parser](https://github.com/paquettg/php-html-parser): An HTML DOM parser. It allows you to manipulate HTML. Find tags on an HTML page with selectors just like jQuery
- [DOM](https://www.php.net/manual/en/intro.dom.php): A built-in PHP extension that allows operations on XML and HTML documents through the DOM API with PHP
- [XML Document Parser PHP](https://github.com/laravie/parser): A framework-agnostic package that provide a simple way to parse XML to array without having to write a complex logic

#### CSV Parsers

- [ParseCsv](https://github.com/parsecsv/parsecsv-for-php): A CSV data parser for PHP

#### JSON Parsers

- [JSON Parser](https://github.com/cerbero90/json-parser): A zero-dependencies lazy parser to read JSON of any dimension and from any source in a memory-efficient way
- [JsonMachine](https://github.com/halaxa/json-machine): An efficient, easy-to-use, and fast PHP JSON stream parser

#### PDF Parsers

- [PdfParser](https://github.com/smalot/pdfparser): A standalone PHP library, provides various tools to extract data from a PDF file

#### Email Parsers

- [EmailReplyParser](https://github.com/willdurand/EmailReplyParser): A PHP library for parsing plain text email content

#### Markdown Parsers

- [CommonMark PHP](https://github.com/thephpleague/commonmark): An highly-extensible PHP Markdown parser which fully supports the CommonMark and GFM specs
- [PHP Markdown](https://github.com/michelf/php-markdown): A parser for Markdown and Markdown Extra derived from the original Markdown.pl by John Gruber
- [Parsedown](https://github.com/erusev/parsedown): A better Markdown parser in PHP

#### YAML Parsers

- [Dallgoot : YAML library for PHP](https://github.com/dallgoot/yaml): A PHP library to load and parse YAML file to PHP datatypes equivalent

#### SQL Parsers

- [PHP-SQL-Parser](https://github.com/greenlion/PHP-SQL-Parser): A pure PHP SQL (non validating) parser w/ focus on MySQL dialect of SQL
- [SQL Parser](https://github.com/phpmyadmin/sql-parser): A validating SQL lexer and parser with a focus on MySQL dialect

#### Office File Parsers

- [SimpleXLSX](https://github.com/shuchkin/simplexlsx): A PHP library to parse and retrieve data from Excel XLSx files

#### Other

- [PHP Domain Parser](https://github.com/jeremykendall/php-domain-parser): Public suffix list based domain parsing implemented in PHP
- [RSS & Atom Feeds for PHP](https://github.com/dg/rss-php): A small and easy-to-use library for consuming RSS and Atom feeds
- [PHP CSS Parser](https://github.com/MyIntervals/PHP-CSS-Parser): A Parser for CSS Files written in PHP. Allows extraction of CSS files into a data structure, manipulation of said structure and output as (optimized) CSS
- [SitemapParser](https://github.com/VIPnytt/SitemapParser): An XML sitemap parser class compliant with the Sitemaps.org protocol
- [robots-txt-parser](https://github.com/bopoda/robots-txt-parser): A PHP class for parse all directives from robots.txt files according to specifications

### Web Scraping

#### Frameworks

- [Crawler](https://github.com/crwlrsoft/crawler): A library for rapid (web) crawler and scraper development
- [Roach](https://github.com/roach-php/core): A complete web scraping toolkit for PHP
- [PHP-Spider](https://github.com/mvdbos/php-spider): A configurable and extensible PHP web spider
- [Embed](https://github.com/oscarotero/Embed): A PHP library to get info from any web service or page
- [PHPScraper](https://github.com/spekulatius/phpscraper): A versatile web-utility for PHP

#### Proxy Integration
- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports  state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]
 
#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]
- [PHP Module for 2Captcha API](https://github.com/2captcha/2captcha-php): A PHP package for easy integration with the API of 2captcha captcha solving service to bypass recaptcha, hcaptcha, funcaptcha, geetest and solve any other captchas
- [captcha-solver-php](https://github.com/metabypass/captcha-solver-php): A PHP-based easy implementation for solving any type of captcha by Metabypass

### Web Automation

#### Browser Automation Frameworks

- [Panther](https://github.com/symfony/panther): A browser testing and web crawling library for PHP and Symfony
- [php-webdriver](https://github.com/facebook/php-webdriver): A PHP client for Selenium/WebDriver protocol
- [chrome-php/chrome](https://github.com/chrome-php/chrome): A library to instrument headless chrome/chromium instances from PHP
- [Mink](https://github.com/minkphp/Mink): PHP web browser emulator abstraction

### Data Export

#### JSON

- [PHP JSON library](https://github.com/josantonius/php-json): A PHP simple library for managing JSON files

#### CSV

- [CSV](https://github.com/thephpleague/csv): A library to ease parsing, writing and filtering CSV in PHP

#### Other

- [mPDF](https://github.com/mpdf/mpdf): A PHP library generating PDF files from UTF-8 encoded HTML
- [PhpSpreadsheet](https://github.com/PHPOffice/PhpSpreadsheet): A pure PHP library for reading and writing spreadsheet files
- [PHPWord](https://github.com/PHPOffice/PHPWord): A A pure PHP library for reading and writing word processing documents
- [PHPPowerPoint](https://github.com/PHPOffice/PHPPowerPoint): A pure PHP library for reading and writing presentations documents

### Data Processing

#### General

- [Stringy](https://github.com/danielstjules/Stringy): A PHP string manipulation library with multibyte support

#### Character Encoding

- [ANSI to HTML5](https://github.com/sensiolabs/ansi-to-html): An ANSI to HTML5 converter

#### Date and Time

- [Brick\DateTime](https://github.com/brick/date-time): A date and time library for PHP

#### Prices

- [Brick\Money](https://github.com/brick/money): A money and currency library for PHP
- [PHP Prices](https://github.com/whitecube/php-prices): A simple PHP library for complex monetary prices management

#### Phone Numbers

- [LibPhoneNumber for PHP](https://github.com/giggsey/libphonenumber-for-php): A PHP version of Google's phone number handling library
- [Brick\PhoneNumber](https://github.com/brick/phonenumber): A phone number library for PHP

#### Units of Measurement

- [PhpUnitsOfMeasure](https://github.com/PhpUnitsOfMeasure/php-units-of-measure): A library for handling physical quantities and the units of measure in which they're represented

#### Slugs

- [Urlify](https://github.com/jbroadway/urlify): A fast PHP slug generator and transliteration library that converts non-ascii characters for use in URLs
- [Slugify](https://github.com/cocur/slugify): A PHP library to convert a string to a slug. Includes integrations for Symfony, Silex, Laravel, Zend Framework 2, Twig, Nette and Latte

#### URLs and Network Addresses

- [Purl](https://github.com/jwage/purl): A a simple Object Oriented URL manipulation library for PHP 7.2+
- [Uri](https://github.com/thephpleague/uri): A PHP package that provides simple and intuitive classes to manage URIs in PHP
- [Url](https://github.com/crwlrsoft/url): A Swiss Army knife for URLs

### Other

#### Multiprocessing

- [amphp/parallel](https://github.com/amphp/parallel): An advanced parallelization library for PHP, enabling efficient multitasking, optimizing resource use, and application responsiveness through multiple CPU threads

#### Even Handling

- [React](https://github.com/reactphp/react) - A library for event-driven, non-blocking I/O with PHP
- [Evenement](https://github.com/igorw/evenement): a very simple event dispatching library for PHP
- [Event](https://github.com/thephpleague/event) - An event library with a focus on domain events

#### Software Automation Management

- [Salt](https://github.com/saltstack/salt): Software to automate the management and configuration of any infrastructure or application at scale
- [Puppet](https://github.com/puppetlabs/puppet): A server automation framework and application

#### Task Scheduling

- [PHP Cron Scheduler](https://github.com/peppeocchi/php-cron-scheduler): A PHP cron job scheduler
- [Crunz](https://github.com/crunzphp/crunz): A PHP-based job scheduler

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: PHP cURL, Guzzle, or Symfony's HttpClient

- **HTML Parser**: Simple Html Dom Parser for PHP, DomCrawler, HTML5-PHP, or DiDOM

#### All-In-One Solution

- Crawler, Roach, or PHP-Spider

### Dynamic Web Pages

- Panther or php-webdriver

## Guides and Tutorials

### General Guides

- [Web Scraping With PHP - Complete Guide](https://brightdata.com/blog/how-tos/web-scraping-php)
- [Web Scraping With Laravel: A Step-by-Step Guide](https://brightdata.com/blog/web-data/web-scraping-with-laravel)
- [Using cURL for Web Scraping](https://brightdata.com/blog/how-tos/how-to-use-curl-for-web-scraping)

### Proxies

- [How to Set Up a Proxy with Guzzle in 2024](https://brightdata.com/blog/how-tos/proxy-with-guzzle)
- [PHP Proxy Server: How to Set Up Proxies in PHP](https://brightdata.com/blog/how-tos/php-proxy-servers)

### HTTP Clients

- [curl GET Request with PHP](https://brightdata.com/blog/how-tos/curl-get-request-with-php)
