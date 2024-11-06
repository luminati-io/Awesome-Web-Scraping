# Perl Web Scraping

This document contains a list of libraries and resources for web scraping in Perl.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [General](#general)
    - [HTTP Clients](#http-clients)
    - [WebSockets](#websockets)
    - [Low Level](#low-level)
    - [Other](#other)
  - [Parsers](#parsers)
    - [HTML Parsers](#html-parsers)
    - [XML Parsers](#xml-parsers)
    - [URL Parsers](#url-parsers)
    - [HTTP Parsers](#http-parsers)
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
    - [JSON](#json)
    - [CSV](#csv)
    - [YAML](#yaml)
    - [Other](#other-3)
  - [Data Processing](#data-processing)
    - [Character Encoding](#character-encoding)
    - [Date and Time](#date-and-time)
    - [Units of Measurement](#units-of-measurement)
    - [Phone Numbers](#phone-numbers)
    - [URLs and Network Addresses](#urls-and-network-addresses)
    - [Languages](#languages)
  - [Other](#other-4)
    - [Multiprocessing](#multiprocessing)
    - [Task Scheduling](#task-scheduling)
- [Popular Web Scraping Stacks](#popular-web-scraping-stacks)
  - [Static Web Pages](#static-web-pages)
    - [HTTP Client + HTML Parser](#http-client-html-parser)
    - [All-In-One Web Scraping Framework](#all-in-one-web-scraping-framework)
  - [Dynamic Web Pages](#dynamic-web-pages)
    - [All-In-One Browser Automation Framework](#all-in-one-browser-automation-framework)
- [Guides and Tutorials](#guides-and-tutorials)

## Libraries

**Note**: All selected libraries are either actively maintained or widely used.

### Network

#### General

- [LWP](https://github.com/libwww-perl/libwww-perl): A collection of Perl modules that provides a simple, consistent application programming interface to the World-Wide Web
- [Plack](https://github.com/plack/Plack): A [PSGI](https://metacpan.org/pod/PSGI) toolkit and server adapters
- [Mojo](https://github.com/mojolicious/mojo): A Perl real-time web framework

#### HTTP Clients

- [LWP::UserAgent](https://metacpan.org/pod/LWP::UserAgent): A class implementing a web user agent
- [HTTP::Tiny](https://github.com/Perl-Toolchain-Gang/HTTP-Tiny): A small, simple, correct HTTP/1.1 client
- [Mojo::UserAgent](https://metacpan.org/pod/Mojo::UserAgent): A non-blocking I/O HTTP and WebSocket user agent
- [WWW::Mechanize](https://github.com/libwww-perl/WWW-Mechanize): A library for handy web browsing in a Perl object
- [WWW::Curl::UserAgent](https://github.com/xing/curl-useragent): A web user agent based on [libcurl](https://curl.se/libcurl/)
- [REST::Client](https://github.com/milescrawford/cpan-rest-client): A simple client for interacting with RESTful HTTP/HTTPS resources
- [HTTP::Async](https://github.com/evdb/HTTP-Async): A library to process multiple HTTP requests in parallel without blocking

#### WebSockets

- [Mojo::WebSocket](https://metacpan.org/pod/Mojo::WebSocket): A library that implements the WebSocket protocol as described in RFC 6455

#### Low Level

- [Net::HTTP](https://github.com/libwww-perl/Net-HTTP): A low-level HTTP connection client

#### Other

- [CGI](https://github.com/leejo/CGI.pm): A library to handle Common Gateway Interface requests and responses

### Parsers

#### HTML Parsers

- [HTML::TreeBuilder](https://github.com/kentfredric/HTML-Tree): A parser that builds a HTML syntax tree
- [HTML::Parser](https://github.com/libwww-perl/HTML-Parser): A collection of modules that parse and extract information from HTML documents
- [Mojo::DOM](https://metacpan.org/pod/Mojo::DOM): A minimalistic HTML/XML DOM parser with CSS selectors
- [HTML::HTML5::Parser](https://github.com/tobyink/p5-html-html5-parser): A Perl library to parse HTML reliably

#### XML Parsers

- [XML::Parser](https://github.com/cpan-authors/XML-Parser): A Perl module for parsing XML documents
- [XML::LibXML](https://github.com/shlomif/perl-XML-LibXML): Perl bindings for [libxml2](https://gitlab.gnome.org/GNOME/libxml2)

#### URL Parsers

- [URI::Info](https://github.com/perlancar/perl-URI-Info): A library to extract various information from a URI (URL)

#### HTTP Parsers

- [HTTP::Entity::Parser](https://github.com/kazeburo/HTTP-Entity-Parser): A PSGI compliant HTTP entity parser
- [HTTP::Parser::XS](https://github.com/kazuho/p5-http-parser-xs): A fast, primitive HTTP request parser
- [Plack::HTTPParser](https://metacpan.org/pod/Plack::HTTPParser): A library to parse HTTP headers
- [HTTP::Body](https://metacpan.org/pod/HTTP::Body): An HTTP body parser
- [HTTP::Parser::XS](https://github.com/kazuho/p5-http-parser-xs): A fast, primitive HTTP request parser
- [HTTP::Parser](https://metacpan.org/pod/HTTP::Parser): A library to parse HTTP/1.1 requests into HTTP::Request/Response objects
- [HTTP::Link::Parser](https://github.com/tobyink/p5-http-link-parser): A library to parse HTTP "Link" headers
- [HTTP::MultiPartParser](https://github.com/chansen/p5-http-multipartparser): A low-level API for processing MultiPart MIME data streams

#### Email Parsers

- [Email::Address::XS](https://github.com/pali/Email-Address-XS): A library to parse and format RFC 5322 email addresses and groups

#### Markdown Parsers

- [Markdown::Parser](https://gitlab.com/jackdeguest/Markdown-Parser): A Markdown parser only

#### SQL Parsers

- [SQL::Parser](https://github.com/perl5-dbi/SQL-Statement): SQL parsing and processing engine

#### Other

- [HTML::TreeBuilder::XPath](https://metacpan.org/pod/HTML::TreeBuilder::XPath): A library to add XPath support to HTML::TreeBuilder
- [HTML::TreeBuilder::LibXML]: A HTML::TreeBuilder and XPath compatible interface with libxml
- [WWW::RobotRules](https://github.com/gisle/www-robotrules): A module to parses robots.txt files as specified in "[A Standard for Robot Exclusion](http://www.robotstxt.org/wc/norobots.html)"
- [XML::RSS::LibXML](https://github.com/lestrrat-p5/XML-RSS-LibXML): A library that uses XML::LibXML (libxml2) for parsing RSS
- [WWW::Sitemap::XML](https://github.com/ajgb/www-sitemap-xml): A library to read and write sitemap XML files as defined at Sitemaps.org

### Web Scraping

#### Frameworks

- [Scrappy](https://metacpan.org/pod/Scrappy): A powerful web spidering, scraping, creeping crawling framework
- [Web::Query](https://github.com/tokuhirom/Web-Query): Yet another scraping library like jQuery
- [WWW::Scraper](https://metacpan.org/pod/WWW::Scraper): A framework for scraping results from search engines

#### Proxy Integration

- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]
- [HTTP::Proxy](https://github.com/book/HTTP-Proxy): A pure Perl HTTP proxy
- [Net::Proxy](https://github.com/book/Net-Proxy): A framework for proxying network connections in many ways

#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]

### Web Automation

#### Browser Automation Frameworks

- [WWW::Mechanize::Chrome](https://github.com/Corion/WWW-Mechanize-Chrome): A library to automate the Chrome browser
- [Playwright](https://github.com/teodesian/playwright-perl): Perl bindings for [Playwright](https://playwright.dev/)
- [Selenium::Edge](https://github.com/teodesian/Selenium-Remote-Driver): Perl bindings to the Selenium Webdriver server
- [Firefox::Marionette](https://github.com/david-dick/firefox-marionette): A library to automate the Firefox browser with the Marionette protocol
- [WWW::Selenium](https://github.com/lukec/cpan-selenium-rc-perl): Perl Client for the Selenium Remote Control test tool

#### Tools and Plugins

- [Firefox::Marionette::Extension::Stealth](): A Stealth extension for Firefox::Marionette

#### Other

- [Chrome::DevToolsProtocol](Chrome::DevToolsProtocol): An asynchronous dispatcher for the DevTools protocol
- [JavaScript::SpiderMonkey](https://github.com/thomasbusch/perl-javascript-spidermonkey): A Perl interface to the [SpiderMonkey](https://spidermonkey.dev/) JavaScript engine

### Data Export

#### JSON

- [JSON](https://github.com/makamaka/JSON): A Perl implementation of a JSON encoder/decoder
- [JSON:PP](https://github.com/makamaka/JSON-PP): A pure Perl JSON decoder/encoder
- [JSON::XS](https://metacpan.org/pod/JSON::XS): JSON serialising/deserialising, done correctly and fast
- [Geo::JSON](https://github.com/mjemmeson/Geo-JSON): A Perl OO interface for GeoJSON
- [JSON::Syck](https://metacpan.org/pod/JSON::Syck): A YAML-based implementation of JSON parsing and generation

#### CSV

- [Text::CSV](https://github.com/makamaka/Text-CSV): Comma-separated values manipulator (using XS or PurePerl)

#### YAML

- [YAML::XS](https://github.com/ingydotnet/yaml-libyaml-pm): A Perl YAML serialization module using XS and [libyaml](https://github.com/yaml/libyaml)
- [YAML](https://github.com/ingydotnet/yaml-pm): A YAML Perl module
- [YAML::PP](https://github.com/perlpunk/YAML-PP-p5): A YAML 1.2 processor in Perl
- [YAML::Syck](https://metacpan.org/pod/YAML::Syck): A fast and lightweight YAML loader and dumper
- [YAML::Tiny](https://github.com/Perl-Toolchain-Gang/YAML-Tiny): A library to read/write YAML files with as little code as possible

#### Other

- [Excel::Writer::XLSX](https://github.com/jmcnamara/excel-writer-xlsx): A Perl module to create Excel XLSX files
- [Pod::Markdown](https://github.com/rwstauner/Pod-Markdown): A library to convert POD to Markdown

### Data Processing

#### Character Encoding

- [PerlIO::encoding](https://metacpan.org/pod/PerlIO::encoding): A built-in library to open a filehandle with a transparent encoding filter
- [Encoding::FixLatin](https://github.com/grantm/encoding-fixlatin): A library that takes mixed encoding input and produces UTF-8 output

#### Date and Time

- [DateTime](https://github.com/houseabsolute/DateTime.pm): A date and time object for Perl
- [Mojo::Date](https://metacpan.org/pod/Mojo::Date): A library that implements HTTP date and time functions, based on RFC 7230, RFC 7231 and RFC 3339
- [HTTP::Date](https://github.com/libwww-perl/HTTP-Date): A module that provides functions that deal the date formats used by the HTTP protocol
- [Date::Manip::Date](https://github.com/SBECK-github/Date-Manip): A library that provides methods for working with dates
- [APR::Date](https://metacpan.org/dist/mod_perl/view/docs/api/APR/Date.pod): Perl API for APR date manipulating functions
- [Date::Calc](https://metacpan.org/dist/Date-Calc/view/lib/Date/Calc.pod): A library for Gregorian calendar date calculations

#### Units of Measurement

- [Class::Measure::Length](https://github.com/bluefeet/Class-Measure): A library to create, compare, and convert units of measurement

#### Phone Numbers

- [Number::Phone](https://github.com/DrHyde/perl-modules-Number-Phone): A large suite of perl modules for parsing and dealing with phone numbers

#### URLs and Network Addresses

- [Mojo::URL](https://github.com/mojolicious/mojo): A library that implements a subset of RFC 3986, RFC 3987 and the URL Living Standard for Uniform Resource Locators with support for IDNA and IRIs
- [URI](https://github.com/libwww-perl/URI): A libray for uniform resource identifiers (absolute and relative)
- [URI::XS](https://metacpan.org/dist/URI-XS/view/lib/URI/XS.pod): A fast URI framework, compatible with classic URI, with C++ interface
- [URL::Encode](https://github.com/chansen/p5-url-encode): A library for encoding and decoding of application/x-www-form-urlencoded encoding

#### Languages

- [Text::Unaccent](https://metacpan.org/pod/Text::Unaccent): A library to remove accents from a string

### Other

#### Multiprocessing

- [MCE](https://github.com/marioroy/mce-perl): A many-core engine for Perl providing parallel processing capabilities
- [Parallel::ForkManager](https://github.com/dluxhu/perl-parallel-forkmanager): A simple parallel processing fork manager
- [Parallel::Runner](https://github.com/exodist/Parallel-Runner): An object to manage running things in parallel processes

#### Task Scheduling

- [Schedule::Cron](https://github.com/NicholasBHubbard/schedule-cron): A cron-like scheduler for Perl subroutines

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: LWP::UserAgent, HTTP::Tiny, Mojo::UserAgent, or WWW::Mechanize
- **HTML Parser**: HTML::TreeBuilder, HTML::Parser, or Mojo::DOM

#### All-In-One Web Scraping Framework

- Scrappy or Web::Query

### Dynamic Web Pages

#### All-In-One Browser Automation Framework

- WWW::Mechanize::Chrome, Playwright, or Firefox::Marionette

## Guides and Tutorials

- [Web Scraping with Perl – Step-By-Step Guide](https://brightdata.com/blog/web-data/web-scraping-with-perl)
