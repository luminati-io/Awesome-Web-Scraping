# Java Web Scraping

This document contains a list of libraries and resources for web scraping in Java.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [HTTP and WebSocket Clients](#http-and-websocket-clients)
    - [WebSockets](#websockets)
    - [Low Level](#low-level)
  - [Parsers](#parsers)
    - [General](#general)
    - [HTML Parsers](#html-parsers)
    - [XML Parsers](#xml-parsers)
    - [URL Parsers](#url-parsers)
    - [CSV Parsers](#csv-parsers)
    - [JSON Parsers](#json-parsers)
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
    - [Other](#other-1)
  - [Data Processing](#data-processing)
    - [General](#general-1)
    - [Character Encoding](#character-encoding)
    - [JSON](#json)
    - [Date and Time](#date-and-time)
    - [Prices](#prices)
    - [Phone Numbers](#phone-numbers)
    - [Slugs](#slugs)
    - [Languages](#languages)
  - [Other](#other-2)
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

**Note**: All selected libraries are either actively maintained or widely used.

### Network

#### HTTP and WebSocket Clients

- [HttpClient](https://docs.oracle.com/en/java/javase/23/docs/api/java.net.http/java/net/http/HttpClient.html): A built-in Java 11 HTTP client to send requests and retrieve their responses
- [HttpURLConnection](https://docs.oracle.com/en/java/javase/23/docs/api/java.base/java/net/HttpURLConnection.html): A built-in Java class to make a single request to an HTTP server
- [HttpsURLConnection](https://docs.oracle.com/en/java/javase/23/docs/api/java.base/javax/net/ssl/HttpsURLConnection.html): A built-in Java class that extends HttpURLConnection with HTTPS-specific features
- [Apache HttpClient](https://github.com/apache/httpcomponents-client): A synchronous HTTP and WebSocket client library for Java
- [Apache AsyncHttpClient](https://github.com/AsyncHttpClient/async-http-client): An asynchronous HTTP and WebSocket client library for Java
- [OkHttp](https://github.com/square/okhttp): A meticulous HTTP client for the JVM, Android, and GraalVM
- [Jetty HttpClient](https://github.com/jetty/jetty.project): An HTTP Client that supports HTTP/2, HTTP/1.1, HTTP/1.0, websocket, servlets, and more
- [Google HTTP Client Library For Java](https://github.com/googleapis/google-http-java-client): A flexible, efficient, and powerful Java library for accessing any resource on the web via HTTP
- [Retrofit](https://github.com/square/retrofit): A type-safe HTTP client for Android and the JVM

#### WebSockets

- [WebSocket](https://docs.oracle.com/en/java/javase/23/docs/api/java.net.http/java/net/http/WebSocket.html): A built-in Java WebSocket client
- [Java-WebSocket](https://github.com/TooTallNate/Java-WebSocket): A barebones WebSocket client and server implementation written in 100% Java

#### Low Level

- [pcap4j](https://github.com/kaitoy/pcap4j): A Java library for capturing, crafting, and sending packets

### Parsers

#### General

- [Apache Tika](https://github.com/apache/tika): A toolkit to detect and extract metadata and text from over a thousand different file types (such as PPT, XLS, and PDF)
- [Jackson Text Dataformats](https://github.com/FasterXML/jackson-dataformats-text): A uber-project for (some) standard Jackson textual format backends: CSV, properties, yaml

#### HTML Parsers

- [jsoup](https://github.com/jhy/jsoup): A Java HTML parser, built for HTML editing, cleaning, scraping, and XSS safety
- [HtmlCleaner](https://htmlcleaner.sourceforge.net/): An open-source HTML parser written in Java
- [JFiveParse](https://github.com/digitalfondue/jfiveparse): A Java HTML 5 compliant parser

#### XML Parsers

- [JAXP](https://docs.oracle.com/en/java/javase/23/docs/api/java.xml/module-summary.html#JAXP): Built-in Java APIs for XML processing

#### URL Parsers

- [URI](https://docs.oracle.com/en/java/javase/23/docs/api/java.base/java/net/URI.html): A built-in Java API for normalizing, resolving, and relativizing URI instances

#### CSV Parsers

- [Apache Commons CSV](https://github.com/apache/commons-csv): A library that provides a simple interface for reading and writing CSV files of various types

#### JSON Parsers

- [JSON Path](https://github.com/json-path/JsonPath): A Java DSL for reading JSON documents

#### Email Parsers

- [Angus Mail](https://github.com/eclipse-ee4j/angus-mail): A library that provides a platform-independent and protocol-independent framework to build mail and messaging applications
- [Apache Commons Email](https://github.com/apache/commons-email): A library that provides an API for sending email, simplifying the JavaMail API

#### Markdown Parsers

- [Flexmark](https://mvnrepository.com/artifact/com.vladsch.flexmark/flexmark-all): A CommonMark/Markdown Java parser with source level AST. CommonMark 0.28, emulation of: pegdown, kramdown, markdown.pl, MultiMarkdown. With HTML to MD, MD to PDF, MD to DOCX conversion modules
- [CommonMark](https://github.com/commonmark/commonmark-java): A Java library for parsing and rendering CommonMark (Markdown)

#### YAML Parsers

- [SnakeYAML](https://bitbucket.org/snakeyaml/snakeyaml): A complete YAML 1.1 processor for the JVM

#### SQL Parsers

- [JSqlParser](https://github.com/JSQLParser/JSqlParser): A library to parse an SQL statement and translate it into a hierarchy of Java classes

#### Office File Parsers

- [Apache POI](https://github.com/apache/poi): A Java API to access Microsoft format files

#### Other

- [Rome](https://github.com/rometools/rome): A Java library for RSS and Atom feeds
- [uap-java](https://github.com/ua-parser/uap-java): The Java implementation of [ua-parser](https://github.com/faisalman/ua-parser-js)
- [Yauaa](https://github.com/nielsbasjes/yauaa): Yet another User-Agent analyzer

### Web Scraping

#### Frameworks

- [Apache Nutch](https://github.com/apache/nutch): An extensible and scalable web crawler
- [WebMagic](https://github.com/code4craft/webmagic): A scalable web crawler framework for Java
- [Jaunt](https://jaunt-api.com/): A Java library for web-scraping, web-automation and JSON querying
- [ACHE Focused Crawler](https://github.com/ViDA-NYU/ache): A web crawler for domain-specific search
- [Gecco](https://github.com/xtuhcy/gecco): An easy-to-use lightweight web crawler
- [StormCrawler](https://github.com/DigitalPebble/storm-crawler): A scalable, mature and versatile web crawler based on Apache Storm

#### Proxy Integration
- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports  state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]

#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver
  that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]

### Web Automation

#### Browser Automation Frameworks

- [Selenium](https://github.com/SeleniumHQ/selenium): A browser automation framework and ecosystem
- [Playwright](https://github.com/microsoft/playwright-java): The Java version of the [Playwright](https://playwright.dev/) testing and automation library
- [HtmlUnit](https://htmlunit.sourceforge.io/): A GUI-less browser for Java programs that models HTML documents and provides an API that allows you to invoke pages, fill out forms, click links, etc
- [Jauntium](https://jauntium.com/): A Java library that allows you to easily automate Chrome, Firefox, Safari, Edge, IE, and other modern web browers

#### Other

- [WebDriverManager](https://github.com/bonigarcia/webdrivermanager): A library that provides automated driver management and other helper features for Selenium WebDriver in Java

### Data Processing

#### General

- [Jackson](https://github.com/FasterXML/jackson): A suite of data-processing tools for Java (and the JVM platform), including the flagship streaming JSON parser / generator library, matching data-binding library (POJOs to and from JSON) and additional data format modules to process data encoded in Avro, BSON, CBOR, CSV, Smile, (Java) Properties, Protobuf, TOML, XML or YAML; and even the large set of data format modules to support data types of widely used data types such as Guava, Joda, PCollections and many, many more (see below)


#### Character Encoding

- [Charset](https://docs.oracle.com/en/java/javase/23/docs/api/java.base/java/nio/charset/Charset.html): A built-in Java class that defines charsets, decoders, and encoders, for translating between bytes and Unicode characters
- [Apache Commons Codec](https://commons.apache.org/proper/commons-codec/): A library that contains encoders and decoders for various formats such as Base16, Base32, Base64, digest, and Hexadecimal

#### JSON

- [JSON](https://github.com/stleary/JSON-java): A reference implementation of a JSON package in Java

#### Date and Time

- [LocalDate](https://docs.oracle.com/en/java/javase/23/docs/api/java.base/java/time/LocalDate.html): A built-in Java class that becomes an immutable date-time object representing a date
- [LocalTime](https://docs.oracle.com/en/java/javase/23/docs/api/java.base/java/time/LocalTime.html): A built-in Java class that becomes an immutable date-time object representing a time
- [Jode-Time](https://github.com/JodaOrg/joda-time): The widely used replacement for the Java date and time classes prior to Java SE 8

#### Prices

- [JSR 354](https://github.com/JavaMoney/jsr354-api): A library that provides an API for representing, transporting, and performing comprehensive calculations with money and currency

#### Phone Numbers

- [libphonenumber](https://github.com/google/libphonenumber): A library for parsing, formatting, and validating international phone numbers

#### Slugs

- [Slugify](https://github.com/slugify/slugify): As mall utility library for generating speaking URLs

#### Languages

- [Apache Commons Lang](https://commons.apache.org/proper/commons-lang/): A library that provides a host of helper utilities for the java.lang API, notably String manipulation methods, basic numerical methods, object reflection, concurrency, creation and serialization and System properties

### Other

#### Task Scheduling
- [Wisp](https://github.com/Coreoz/Wisp): A simple Java scheduler library with a minimal footprint and a straightforward API

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: HttpClient, Apache HttpClient, Apache AsyncHttpClient, OkHttp, Jetty HttpClient, Google HTTP Client Library For Java, or Retrofit

- **HTML Parser**: Jsoup or HtmlCleaner

#### All-In-One Solution

- Jsoup

### Dynamic Web Pages

- Selenium, Playwright or HtmlUnit

## Guides and Tutorials

### General Guides

- [Web scraping with Java - Complete Guide 2024](https://brightdata.com/blog/how-tos/java-web-scraping)
- [Web Scraping in Java With Jsoup: A Step-By-Step Guide](https://brightdata.com/blog/how-tos/web-scraping-with-jsoup)

### Comparisons

- [Java vs Python - Comparison Guide](https://brightdata.com/blog/web-data/java-vs-python)
- [Java vs C# for Web Scraping](https://brightdata.com/blog/web-data/java-vs-c-sharp)
- [Playwright vs. Selenium Comparison 2024](https://brightdata.com/blog/web-data/playwright-vs-selenium)
