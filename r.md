# R Web Scraping

This document contains a list of libraries and resources for web scraping in R.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [HTTP Clients and WebSockets](#http-clients-and-websockets)
    - [WebSockets](#websockets)
    - [Other](#other)
  - [Parsers](#parsers)
    - [HTML/XML Parsers](#htmlxml-parsers)
    - [URL Parsers](#url-parsers)
    - [CSV Parsers](#csv-parsers)
    - [Date and Time Parsers](#date-and-time-parsers)
    - [PDF Parsers](#pdf-parsers)
    - [Markdown Parsers](#markdown-parsers)
    - [YAML Parsers](#yaml-parsers)
    - [SQL Parsers](#sql-parsers)
    - [Office File Parsers](#office-file-parsers)
    - [Other](#other-1)
  - [Web Scraping](#web-scraping)
    - [Frameworks](#frameworks)
    - [Tools and Plugins](#tools-and-plugins)
    - [Proxy Integration](#proxy-integration)
    - [CAPTCHA Solving](#captcha-solving)
    - [User-Agent Spoofing](#user-agent-spoofing)
    - [Other](#other-2)
  - [Web Automation](#web-automation)
    - [Browser Automation Frameworks](#browser-automation-frameworks)
    - [Tools and Plugins](#tools-and-plugins-1)
    - [Other](#other-3)
  - [Data Export](#data-export)
    - [JSON](#json)
    - [CSV](#csv)
    - [Other](#other-4)
  - [Data Processing](#data-processing)
    - [General](#general)
    - [Tabular Data](#tabular-data)
    - [Character Encoding](#character-encoding)
    - [Date and Time](#date-and-time)
    - [Phone Numbers](#phone-numbers)
    - [Other](#other-5)
  - [Other](#other-6)
    - [Multiprocessing](#multiprocessing)
    - [Task Scheduling](#task-scheduling)
  * [Popular Web Scraping Stacks](#popular-web-scraping-stacks)
    - [Static Web Pages](#static-web-pages)
      - [HTTP Client + HTML Parser](#http-client-html-parser)
      - [All-In-One Web Scraping Framework](#all-in-one-web-scraping-framework)
    - [Dynamic Web Pages](#dynamic-web-pages)
      - [All-In-One Browser Automation Framework](#all-in-one-browser-automation-framework)
  * [Guides and Tutorials](#guides-and-tutorials)

## Libraries

**Note**: All selected libraries are either actively maintained or widely used.

### Network

#### HTTP Clients

- [httr2](https://github.com/r-lib/httr2): An R libary to make HTTP requests and process their responses. A modern reimagining of httr
- [crul](https://github.com/ropensci/crul): An [R6](https://r6.r-lib.org/) based HTTP client for R (for developers)
- [RCurl](https://cran.r-project.org/web/packages/RCurl/index.html): A wrapper for [libcurl](https://curl.se/libcurl/)
- [request](https://github.com/sckott/request): HTTP requests DSL for R
- [httpRequest](https://cran.r-project.org/web/packages/httpRequest/index.html): An R library to HTTP request protocols. Implements the GET, POST and multipart POST request
- [routr](https://github.com/thomasp85/routr): Routing of web requests in R

#### WebSockets

- [websocket](https://github.com/rstudio/websocket): WebSocket client for R
- [httpuv](https://github.com/rstudio/httpuv): HTTP and WebSocket server package for R

#### Other

- [fauxpas](https://sckott.github.io/fauxpas/): An R library that provides HTTP error helpers
- [reqres](https://github.com/thomasp85/reqres): Powerful classes for HTTP requests and responses
- [tryr](https://github.com/analythium/tryr): Client/Server error handling for HTTP APIs
- [base64url](https://github.com/mllg/base64url): A fast and url-safe base64 encoder and decoder for R

### Parsers

#### HTML/XML Parsers

- [xml2](https://github.com/r-lib/xml2): R bindings to [libxml2](https://gitlab.gnome.org/GNOME/libxml2)
- [XiMpLe](https://cran.r-project.org/web/packages/XiMpLe/index.html): A library that provides a simple XML tree parser/generator
- [XML]: Tools for parsing and generating XML within R and [S-Plus](https://en.wikipedia.org/wiki/S-PLUS)
- [xml2relational](https://github.com/jsugarelli/xml2relational/): A library for converting XML documents into relational data models
- [xmlconvert](https://github.com/jsugarelli/xmlconvert/): A library for comfortably converting XML documents to dataframes and vice versa
- [xmlr](https://github.com/Alipsa/xmlr): XML dom package for R similar to [jdom](https://github.com/hunterhacker/jdom) implemented using [Reference Classes](http://adv-r.had.co.nz/R5.html)

#### URL Parsers

- [adaR](https://github.com/gesistsa/adaR): A wrapper for [ada-url](https://github.com/ada-url/ada), a WHATWG-compliant and fast URL parser written in modern C++

#### CSV Parsers

- [csvread](https://github.com/jabiru/csvread): A fast and specialized CSV file loader
- [easycsv](https://github.com/bogind/easycsv): An R package for easy data loading from multiple tables

#### Date and Time Parsers

- [parsedate](https://github.com/gaborcsardi/parsedate): An R package to parse dates given in arbitrary formats

#### PDF Parsers

- [pdfsearch](https://github.com/lebebr01/pdfsearch): A libeary to search PDF files for keywords
- [pdftools](https://github.com/ropensci/pdftools): Tools for text extraction, rendering, and converting of PDF documents
- [tabulapdf](https://github.com/ropensci/tabulapdf/): R bindings for [Tabula](https://github.com/tabulapdf/tabula) PDF table extractor library
- [pdf](https://github.com/expersso/pdftables): A library for programmatic conversion of PDF tables with R
- [Rpoppler](https://cran.r-project.org/web/packages/Rpoppler/index.html): PDF tools based on [Poppler](https://poppler.freedesktop.org/)
- [staplr](https://cran.r-project.org/web/packages/staplr/index.html): A toolkit for PDF files that provides functions to manipulate PDF files
- [pdfminer](https://cran.r-project.org/web/packages/pdfminer/index.html): An R library that provides an interface to [PDFMiner](https://github.com/pdfminer/pdfminer.six), a Python package for extracting information from PDF-files

#### Markdown Parsers

- [marquee](https://github.com/r-lib/marquee): A Markdown parser and renderer for R Graphics
- [parsemd](https://github.com/rundel/parsermd): A library to extract the content of an R Markdown file to allow for programmatic interactions with the document’s contents
- [md4r](https://cran.r-project.org/web/packages/md4r/index.html): A Markdown parser implemented using the [MD4C](https://github.com/mity/md4c) library

#### YAML Parsers

- [yum](https://gitlab.com/r-packages/yum): Utilities to extract and process YAML fragments

#### SQL Parsers

- [RSqlParser](https://cran.r-project.org/web/packages/RSqlParser/index.html): A parser for SQL statements
- [queryparser](https://github.com/ianmcook/queryparser): A library to translate SQL queries into R expressions
- [sqlparseR]: A wrapper for the Python module [sqlparse](https://github.com/andialbrecht/sqlparse)

#### Office File Parsers

- [readxl](https://github.com/tidyverse/readxl): A library to read excel files (.xls and .xlsx) into R
- [readxlsb](https://github.com/velofrog/readxlsb): A library to import Excel binary (.xlsb) spreadsheets into R
- [exceldata](https://cran.r-project.org/web/packages/exceldata/index.html): A library to streamline data import, cleaning, and recoding from Excel
- [modgetxl](https://cran.r-project.org/web/packages/modgetxl/index.html): A shiny module for reading Excel sheets

#### Other

- [humaniformat](https://github.com/ironholds/humaniformat/): A human name parser
- [parcr](https://github.com/SystemsBioinformatics/parcr): Construct parser combinators in R
- [qmrparser](https://cran.r-project.org/web/packages/qmrparser/index.html): A parser combinator in R that provides basic functions for building parsers
- [robotstxt](https://github.com/ropensci/robotstxt): An R library for parsing and checking robots.txt files
- [r-optparse](https://github.com/trevorld/r-optparse): A command-line optional argument parser
- [configr](https://github.com/Miachol/configr): A library that implements the JSON, INI, YAML and TOML parser
- [xmlparsedata](https://github.com/r-lib/xmlparsedata): R code parse data as an XML tree

### Web Scraping

#### Frameworks

- [rvest](https://github.com/tidyverse/rvest): Simple web scraping for R
- [Rcrawler](https://github.com/salimk/Rcrawler/): An R web crawler and scraper
- [ralger](https://github.com/feddelegrand7/ralger): A library that makes it easy to scrape a website. Built on the shoulders of titans: rvest, xml2
- [scrapeR](https://cran.r-project.org/web/packages/scrapeR/index.html): Functions to fetch and extract text content from specified web pages

#### Tools and Plugins

- [scraEP](https://cran.r-project.org/web/packages/scraEP/index.html): Tools for scraping information from webpages and other XML contents, using XPath or CSS selectors

#### Proxy Integration

- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]
- [getProxy](https://github.com/selesnow/getProxy): An R library to get a free proxy IP and port in R
- [ip2proxy](https://cran.r-project.org/web/packages/ip2proxy/index.html): An R library that enables user to find the IP addresses which are used as VPN anonymizer, open proxies, web proxies and Tor exits
- [r.proxy](https://github.com/xiayh17/r.proxy): A library to set a proxy in an R console

#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]

#### User-Agent Spoofing

- [Randomuseragent](https://cran.r-project.org/web/packages/Randomuseragent/index.html): A library for filtering and randomly sampling real User-Agent strings

#### Other

- [heapsofpapers](https://github.com/RohanAlexander/heapsofpapers): A library to easily download heaps of PDF and CSV files
- [antiword](https://cran.r-project.org/web/packages/antiword/index.html): A library to extract text from Microsoft Word documents
- [tidyrss](https://github.com/RobertMyles/tidyrss): An R package for extracting tidy dataframes from RSS, Atom and JSON feeds
- [getwiki](https://cran.r-project.org/web/packages/getwiki/index.html): An R wrapper for Wikipedia data
- [tidywikidatar](https://github.com/EDJNet/tidywikidatar): A library to explore Wikidata through Tidy dataframes

### Web Automation

#### Browser Automation Frameworks

- [RSelenium](https://docs.ropensci.org/RSelenium/): R bindings for [Selenium WebDriver](https://www.selenium.dev/)
- [chromote](https://github.com/rstudio/chromote): A Chrome remote interface for R
- [hayalbaz](https://github.com/rundel/hayalbaz): An R package provides a puppeteer inspired interface to the Chrome Devtools Protocol using chromote
- [selenium-r](https://github.com/ashbythorpe/selenium-r): A low-level browser automation interface

#### Tools and Plugins

- [parsel](https://github.com/till-tietz/parsel): A tool for parallel execution of RSelenium

#### Other

- [selenider](https://github.com/ashbythorpe/selenider): A concise, lazy, and reliable wrapper for chromote and selenium

### Data Export

#### JSON

- [jsonlite](https://github.com/jeroen/jsonlite): A Robust, high performance JSON parser and generator for R
- [geojson](https://github.com/ropensci/geojson): GeoJSON classes for R
- [yyjsonr](https://github.com/coolbutuseless/yyjsonr): A fast JSON package for R
- [rapidjsonr](https://cran.r-project.org/web/packages/rapidjsonr/index.html): A library to provide JSON parsing capability through the [Rapidjson](https://github.com/Tencent/rapidjson/) C++ header-only library
- [RJSONIO](https://cran.r-project.org/web/packages/RJSONIO/index.html): A package that allows conversion to and from data in Javascript object notation (JSON) format
- [rjson](https://cran.r-project.org/web/packages/rjson/index.html): A library that converts R object into JSON objects and vice-versa

#### CSV

- [csv](https://cran.r-project.org/web/packages/csv/index.html): A library to read and write CSV files with selected conventions
- [csvwr](https://github.com/Robsteranium/csvwr): A library to read and write CSVW (i.e., CSV tables and JSON metadata)
- [csvy](https://github.com/leeper/csvy): A library that provides for import from and export to the CSVY file format

#### Other

- [cleanrmd](https://github.com/gadenbuie/cleanrmd): Clean class-less R Markdown HTML documents
- [r-yaml](https://github.com/vubiostat/r-yaml/): An R package for converting objects to and from YAML
- [df2yaml](https://cran.r-project.org/web/packages/df2yaml/index.html): A library that converts dataframes to YAML
- [xlsx](https://github.com/colearendt/xlsx): An R package to interact with Excel files using the [Apache POI Java](https://poi.apache.org/) library
- [writexl](https://cran.r-project.org/web/packages/writexl/index.html): A zero-dependency dataframe to xlsx exporter based on [libxlsxwriter](https://libxlsxwriter.github.io)

### Data Processing

#### General

- [tidyverse](https://github.com/tidyverse/tidyverse): Easily install and load packages from the tidyverse

#### Tabular Data

- [tinytable](https://github.com/vincentarelbundock/tinytable): Simple and customizable tables in R

#### Character Encoding

- [utf8](https://cran.r-project.org/web/packages/utf8/index.html): A library to process and print UTF-8 encoded international text
- [base64](https://cran.r-project.org/web/packages/base64/index.html): A Base64 encoder and decoder

#### Date and Time

- [lubridate](https://github.com/tidyverse/lubridate): A library that makes working with dates in R just that little bit easier
- [date](https://cran.r-project.org/web/packages/date/index.html): Functions for handling dates
- [datefixR](https://github.com/ropensci/datefixR): A library to standardize dates in different formats or with missing data

#### Phone Numbers

- [dialr](https://github.com/socialresearchcentre/dialr): A library that parse, format, and validate international phone numbers in R

#### Other

- [geojsonR](https://github.com/mlampros/geojsonR): A GeoJSON processing toolkit
- [jsonStrings](https://github.com/stla/jsonStrings): A library to manipulate JSON strings in R
- [excel.link](https://github.com/gdemin/excel.link): A library for convenient data exchange between R and Microsoft Excel
- [officer](https://github.com/davidgohel/officer): A package that lets R users manipulate Word (.docx) and PowerPoint (.pptx) documents

### Other

#### Multiprocessing

- [parallel](https://www.rdocumentation.org/packages/parallel/versions/3.6.2): A built-in R library that provides support for parallel computation, including by forking (taken from package multicore), by sockets (taken from package snow) and random-number generation
- [parallelly](https://github.com/HenrikBengtsson/parallelly): A library for enhancing the parallel package
- [RcppThread](https://github.com/tnagler/RcppThread): A library that provides a C++11-style thread class and thread pool that can safely be interrupted from R

#### Task Scheduling

- [cronR](https://github.com/bnosac/cronR): A simple R package for managing your cron jobs
- [later](https://github.com/r-lib/later): A library to schedule an R function or formula to run after a specified period of time
- [taskscheduleR](https://github.com/bnosac/taskscheduleR): A library to schedule R scripts/processes with the Windows task scheduler
- [sched](https://gitlab.com/cnrgh/databases/r-sched): A library that offers classes and functions to contact web servers while enforcing scheduling rules required by the sites

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: httr2 or RCurl
- **HTML Parser**: xml2

#### All-In-One Web Scraping Framework

- rvest or Rcrawler

### Dynamic Web Pages

#### All-In-One Browser Automation Framework

- RSelenium

## Guides and Tutorials

- [A Hands-On Guide to Web Scraping in R](https://brightdata.com/blog/how-tos/web-scraping-with-r)
