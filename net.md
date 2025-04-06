# .NET Web Scraping

This document contains a list of libraries and resources for web scraping in .NET languages, including C#, F#, and Visual Basic.

## Table of Contents

- [Libraries](#libraries)
  - [Network](#network)
    - [HTTP Clients](#http-clients)
    - [WebSockets](#websockets)
    - [Low Level](#low-level)
  - [Parsers](#parsers)
    - [HTML/XML Parsers](#html-xml-parsers)
    - [URL Parsers](#url-parsers)
    - [CSV Parsers](#csv-parsers)
    - [Text Parsers](#text-parsers)
    - [Date and Time Parsers](#date-and-time-parsers)
    - [PDF Parsers](#pdf-parsers)
    - [HTTP Parsers](#http-parsers)
    - [Email Parsers](#email-parsers)
    - [Markdown Parsers](#markdown-parsers)
    - [SQL Parsers](#sql-parsers)
    - [Office File Parsers](#office-file-parsers)
    - [Other](#other)
  - [Web Scraping](#web-scraping)
    - [Frameworks](#frameworks)
    - [Tools and Plugins](#tools-and-plugins)
    - [Anti-Bot Bypass](#anti-bot-bypass)
    - [Proxy Integration](#proxy-integration)
    - [CAPTCHA Solving](#captcha-solving)
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
    - [Units of Measurement](#units-of-measurement)
    - [Slugs](#slugs)
    - [Languages](#languages)
    - [Other](#other-3)
  - [Other](#other-4)
    - [Task Scheduling](#task-scheduling)
  * [Popular Web Scraping Stacks](#popular-web-scraping-stacks)
    - [Static Web Pages](#static-web-pages)
      - [HTTP Client + HTML Parser](#http-client---html-parser)
      - [All-In-One Web Scraping Framework](#all-in-one-web-scraping-framework)
    - [Dynamic Web Pages](#dynamic-web-pages)
      - [All-In-One Browser Automation Framework](#all-in-one-browser-automation-framework)
  * [Guides and Tutorials](#guides-and-tutorials)
    - [General Guides](#general-guides)
    - [Proxies](#proxies)
    - [Comparisons](#comparisons)

## Libraries

**Note**: All selected libraries are either widely used or actively maintained.

### Network

#### HTTP Clients

- [HttpClient](https://learn.microsoft.com/en-us/dotnet/api/system.net.http.httpclient): A built-in .NET class for sending HTTP requests and receiving HTTP responses from a resource identified by a URI
- [RestSharp](https://github.com/restsharp/RestSharp): A simple REST and HTTP API client for .NET
- [Flurl](https://github.com/tmenier/Flurl): A fluent URL builder and testable HTTP client for .NET
- [Refit](https://github.com/reactiveui/refit): An automatic type-safe REST library for .NET Core, Xamarin and .NET. Heavily inspired by [Square's Retrofit library](https://github.com/square/retrofit), Refit turns your REST API into a live interface
- [RestEasy](https://github.com/canton7/RestEase): An easy-to-use typesafe REST API client library for .NET Standard 1.1 and .NET Framework 4.5 and higher, which is simple and customisable

#### WebSockets

- [WebSocketSharp](https://github.com/sta/websocket-sharp): A C# implementation of the WebSocket protocol client and server
- [Websocket.Client](https://github.com/Marfusios/websocket-client): A .NET/C# WebSocket client library
- [WatsonWebsocket](https://github.com/jchristn/WatsonWebsocket): A simple C# async websocket server and client for reliable transmission and receipt of data
- [WebSocket4Net](https://github.com/kerryjiang/WebSocket4Net): A popular .NET WebSocket client

#### Low Level

- [sharppcap](https://github.com/dotpcap/sharppcap): A fully managed, cross platform (Windows, Mac, Linux) .NET library for capturing packets

### Parsers

#### HTML/XML Parsers

- [AngleSharp](https://github.com/AngleSharp/AngleSharp): The ultimate angle brackets parser library parsing HTML5, MathML, SVG and CSS to construct a DOM based on the official W3C specifications
- [CsQuery](https://github.com/jamietre/CsQuery): A complete CSS selector engine, HTML parser, and jQuery port for C# and .NET 4
- [MariGold.HtmlParser](https://github.com/kannan-ar/MariGold.HtmlParser): A utility to convert an HTML string into the collection of IHtmlNode
- [HtmlPerformanceKit](https://github.com/osjoberg/HtmlPerformanceKit): A fast HTML parser whith a similar API as [XmlReader](https://learn.microsoft.com/en-us/dotnet/api/system.xml.xmlreader)
- [Majestic12HtmlParser](https://www.majestic12.co.uk/projects/html_parser.php): An open source high-performance .NET C# module that was created to parse HTML for links, indexing, and other purposes

#### URL Parsers

- [Uri](https://learn.microsoft.com/en-us/dotnet/api/system.uri): A built-in .NET class that provides an object representation of a uniform resource identifier (URI) and easy access to the parts of the URI

#### CSV Parsers

- [TinyCsvParser](https://github.com/TinyCsvParser/TinyCsvParser): An easy to use, easy to extend and high-performance library for CSV parsing with .NET
- [CsvTextFieldParser](https://github.com/22222/CsvTextFieldParser): A simple CSV parser based on [Microsoft.VisualBasic.FileIO.TextFieldParser](https://learn.microsoft.com/en-us/dotnet/api/microsoft.visualbasic.fileio.textfieldparser)
- [Sep](https://github.com/nietras/Sep/): The world's Fastest .NET CSV Parser. Modern, minimal, fast, zero allocation, reading and writing of separated values (csv, tsv, etc.). Cross-platform, trimmable and AOT/NativeAOT compatible

#### Text Parsers

- [GenericParsing](https://github.com/AndrewRissing/GenericParsing): A C# implementation of a parser for delimited and fixed width format files

#### Date and Time Parsers

- [Chronic.Signed](https://github.com/robertwilczynski/nChronic): A natural language date/time parser ported from Ruby

#### PDF Parsers

- [PdfPig](https://github.com/UglyToad/PdfPig/): A library to read and extract text and other content from PDFs in C# (port of [PDFBox](https://pdfbox.apache.org/))
- [DocNET](https://github.com/GowenGit/docnet): A fast PDF editing and reading library for modern .NET application
- [PdfSharpCore](https://github.com/ststeiger/PdfSharpCore/): A port of the PdfSharp library to .NET Core - largely removed GDI+ (only missing GetFontData - which can be replaced with freetype2)

#### HTTP Parsers

- [HttpMultipartParser](https://github.com/Http-Multipart-Data-Parser/Http-Multipart-Data-Parser): A C# Http Multipart/form-data parser that works correctly on binary data and very large files

#### Email Parsers

- [MimeKit](https://github.com/jstedfast/MimeKit): A .NET MIME creation and parser library with support for S/MIME, PGP, DKIM, TNEF and Unix mbox spools

#### Markdown Parsers

- [Markdig](https://github.com/xoofx/markdig): A fast, powerful, CommonMark compliant, extensible Markdown processor for .NET
- [MarkedNET](https://github.com/alex-titarenko/markednet): A full-featured Markdown parser and compiler, written in C#
- [MarkdownSharp](https://github.com/StackExchange/MarkdownSharp): An open source C# implementation of Markdown processor, used by Stack Overflow

#### SQL Parsers

- [SQLParser](https://github.com/JaCraig/SQLParser): An SQL Parser/Lexer for C#
- [SqlParserCS](https://github.com/TylerBrinks/SqlParser-cs): A friendly SQL parser for .NET
- [TSQL.Parser](https://github.com/bruce-dunwiddie/tsql-parser): A library Written in C# For Parsing SQL Server T-SQL Scripts in .Net

#### Office File Parsers

- [ExcelDataReader](https://github.com/ExcelDataReader/ExcelDataReader): A lightweight and fast library written in C# for reading Microsoft Excel files
- [EPPlus](https://github.com/EPPlusSoftware/EPPlus): Spreadsheets for .NET
- [DocX](https://github.com/xceedsoftware/DocX): A fast and easy to use .NET library that creates or modifies Microsoft Word files without installing Word

#### Other

- [CommandLineParser](https://github.com/commandlineparser/commandline): The best C# command line parser that brings standardized [\*nix getopt style](https://en.wikipedia.org/wiki/Getopt), for .NET. Includes F# support
- [Fizzler](https://github.com/atifaziz/Fizzler): A .NET CSS selector engine
- [Microsoft.Recognizers.Text](https://github.com/Microsoft/Recognizers-Text): A built-in Microsoft library that provides recognition and resolution of numbers, units, date/time, etc. in multiple languages (ZH, EN, FR, ES, PT, DE, IT, TR, HI, NL. Partial support for JA, KO, AR, SV)
- [AngleSharp.Xml](https://github.com/AngleSharp/AngleSharp.Xml): A library to add XML and DTD parsing capabilities to AngleSharp
- [RssParser](https://learn.microsoft.com/en-us/dotnet/api/microsoft.toolkit.parsers.rss.rssparser): A built-in Microsoft library that allows you to parse an RSS content String into RSS Schema
- [FeedReader](https://github.com/arminreiter/FeedReader/): A C# RSS and ATOM Feed reader library. Supports RSS 0.91, 0.92, 1.0, 2.0 and ATOM. Tested with multiple languages and feeds
- [RobotsExclusionTools](https://github.com/TurnerSoftware/RobotsExclusionTools): A "robots.txt" parsing and querying library for .NET
- [SitemapTools](https://github.com/TurnerSoftware/SitemapTools): A sitemap (sitemap.xml) querying and parsing library for .NET

### Web Scraping

#### Frameworks

- [HtmlAgilityPack](https://github.com/zzzprojects/html-agility-pack/): A free and open-source HTML parser written in C# to read/write DOM and supports plain XPATH or XSLT. It is a .NET code library that allows you to parse "out of the web" HTML files
- [ScrapySharp](https://github.com/rflechner/ScrapySharp): A library that has a Web Client able to simulate a real web browser
- [InfinityCrawler](https://github.com/TurnerSoftware/InfinityCrawler): A simple but powerful web crawler library for .NET
- [Abot](https://github.com/sjdirect/abot): A cross platform C# web crawler framework built for speed and flexibility
- [DotnetSpider](https://github.com/dotnetcore/DotnetSpider): A .NET standard web crawling library. It is lightweight, efficient and fast high-level web crawling & scraping framework

#### Tools and Plugins

- [Hazz](https://github.com/atifaziz/Hazz): CSS Selectors (via Fizzler) for HtmlAgilityPack (HAP)
- [HtmlAgilityPack.CssSelector](https://github.com/hcesar/HtmlAgilityPack.CssSelector): An HtmlAgilityPack CSS selector extension

#### Anti-Bot Bypass

- [FlareSolverr](https://github.com/FlareSolverr/FlareSolverrSharp): .NET / Proxy server to bypass Cloudflare protection

#### Proxy Integration

- [Bright Data's proxy services](https://brightdata.com/proxy-types): A proxy network with over 72 million IPs offering premium residential, datacenter, mobile, and ISP proxies. Supports state, country, ZIP, and ASN level targeting across 195 countries. Works with any HTTP client or scraping library [**Bright Data's solution**]
- [Yarp.ReverseProxy](https://www.nuget.org/packages/Yarp.ReverseProxy): A toolkit for developing high-performance HTTP reverse proxy applications

#### CAPTCHA Solving

- [CAPTCHA Solver](https://brightdata.com/products/web-unlocker/captcha-solver): A rapid and automated CAPTCHA solver that can solve challenges from reCAPTCHA, hCaptcha, px_captcha, SimpleCaptcha, GeeTest CAPTCHA, and more [**Bright Data's solution**]
- [CaptchaSharp](https://github.com/openbullet/CaptchaSharp): A .NET universal interface for the Web APIs of all major captcha solving services

### Web Automation

#### Browser Automation Frameworks

- [Microsoft.Playwright](https://github.com/microsoft/playwright-dotnet): A .NET version of the [Playwright](https://playwright.dev/) testing and automation library
- [PuppeteerSharp](https://github.com/hardkoded/puppeteer-sharp): A .NET port of the official [Node.js Puppeteer API](https://pptr.dev/)
- [Selenium.WebDriver](https://github.com/SeleniumHQ/selenium): A browser automation framework and ecosystem
- [Atata](https://github.com/atata-framework/atata): A C#/.NET test automation framework for web
- [Coypu](https://github.com/featurist/coypu): An intuitive, robust browser automation for .NET

#### Tools and Plugins

- [ExtraStealth](https://github.com/Overmiind/Puppeteer-sharp-extra/tree/master/PuppeteerExtraSharp/Plugins/ExtraStealth): A PuppeteerExtraSharp and PlaywrightExtraSharp plugin that applies various evasion techniques to make detection of headless Puppeteer harder
- [AnonymizeUa](https://github.com/Overmiind/Puppeteer-sharp-extra/tree/master/PuppeteerExtraSharp/Plugins/AnonymizeUa): A PuppeteerExtraSharp and PlaywrightExtraSharp plugin to anonymize the user-agent on all pages
- [Recaptcha](https://github.com/Overmiind/Puppeteer-sharp-extra/tree/master/PuppeteerExtraSharp/Plugins/Recaptcha): A PuppeteerExtraSharp and PlaywrightExtraSharp plugin to solve reCAPTCHA automatically
- [BlockResources](https://github.com/Overmiind/Puppeteer-sharp-extra/tree/master/PuppeteerExtraSharp/Plugins/BlockResources): A PuppeteerExtraSharp and PlaywrightExtraSharp plugin to blocks images, documents, etc

#### Other

- [PuppeteerExtraSharp](https://github.com/Overmiind/Puppeteer-sharp-extra): a .NET port of the [Puppeteer Extra Node.js library](https://github.com/berstend/puppeteer-extra)
- [PlaywrightExtraSharp](https://github.com/hardkoded/playwright-sharp): A .NET library based on PuppeteerExtraSharp and [Node.js Playwright Extra](https://github.com/berstend/puppeteer-extra/blob/master/packages/playwright-extra)

### Data Export

#### JSON

- [System.Text.Json](https://learn.microsoft.com/en-us/dotnet/api/system.text.json): A built-in .NET namespace that provides high-performance, low-allocating, and standards-compliant capabilities to process JavaScript Object Notation (JSON)
- [Json.NET](https://github.com/JamesNK/Newtonsoft.Json): A popular high-performance JSON framework for .NET
- [Jil](https://github.com/kevin-montrose/Jil): A fast .NET JSON (de)serializer, built on [Sigil](https://github.com/kevin-montrose/Sigil)

#### CSV

- [CsvHelper](https://github.com/JoshClose/CsvHelper): A library to help reading and writing CSV files
- [FlatFiles](https://github.com/jehugaleahsa/FlatFiles): A library that reads and writes CSV, fixed-length and other flat file formats with a focus on schema definition, configuration and speed
- [CsvExport](https://github.com/jitbit/CsvExport): A very simple CSV-export tool for C#

#### Other

- [YamlDotNet](https://github.com/aaubry/YamlDotNet): A a .NET library for low level parsing and emitting of YAML
- [SharYaml](https://github.com/xoofx/SharpYaml): A .NET library for YAML compatible with CoreCLR
- [Ceras](https://github.com/rikimaru0345/Ceras): A universal binary serializer for a wide variety of scenarios
- [Protobuf.NET](https://github.com/protobuf-net/protobuf-net): A protocol buffers library for idiomatic .NET
- [Bond](https://github.com/Microsoft/bond): A cross-platform framework for working with schematized data. It supports cross-language de/serialization and powerful generic mechanisms for efficiently manipulating data. Bond is broadly used at Microsoft in high scale services
- [Hyperion](https://github.com/akkadotnet/Hyperion): A library for polymorphic serialization for .NET
- [FileHelpers](https://github.com/MarcosMeli/FileHelpers): A free and easy to use .NET library to read/write data from fixed length or delimited records in files, strings or streams

### Data Processing

#### Character Encoding

- [Encoding](https://learn.microsoft.com/en-us/dotnet/api/system.text.encoding): A built-in .NET library to represent a character encoding and convert a string from one encoding to another

#### Date and Time

- [NodaTime](https://github.com/nodatime/nodatime): A better date and time API for .NET

#### Prices

- [NodaMoney](https://github.com/RemyDuijkeren/NodaMoney): A library that treats Money as a first class citizen and handles all the ugly bits like currencies and formatting
- [currency-dotnet](https://github.com/irensaltali/currency-dotnet): Currency API for .Net Core

#### Human Names

- [RandomNameGeneratorLibrary](https://github.com/m4bwav/DotNetRandomNameGenerator): A library to generate random people and place names drawn from freely available US census data

#### Phone Numbers

- [https://github.com/twcclegg/libphonenumber-csharp](libphonenumber-csharp): The Offical C# port of [Google's libphonenumber](https://github.com/googlei18n/libphonenumber)

#### Units of Measurement

- [UnitsNet](https://github.com/angularsen/UnitsNet): A library that makes life working with units of measurement just a little bit better

#### Slugs

- [Slugify.Core](https://github.com/ctolkien/Slugify): A simple slug / clean URL generator helper for Microsoft .NET framework / .NET Standard

#### Languages

- [Diacritics.NET](https://github.com/thomasgalliker/Diacritics.NET): A library that finds and replaces diacritics in strings

#### Other

- [Humanizer](https://github.com/Humanizr/Humanizer): A library that meets all your .NET needs for manipulating and displaying strings, enums, dates, times, timespans, numbers and quantities
- [AnyAscii](https://github.com/anyascii/anyascii): A library for Unicode to ASCII transliteration

### Other

#### Task Scheduling

- [Quartz](https://github.com/quartznet/quartznet): An enterprise job scheduler for .NET
- [FluentScheduler](https://github.com/fluentscheduler/FluentScheduler): An automated job scheduler with fluent interface for the .NET platform
- [HangFire](https://github.com/HangfireIO/Hangfire): An easy way to perform background job processing in .NET and .NET Core applications. No Windows Service or separate process required
- [TaskScheduler](https://github.com/dahall/taskscheduler): A .NET wrapper for the Windows Task Scheduler. It aggregates the multiple versions, provides an editor and allows for localization

## Popular Web Scraping Stacks

### Static Web Pages

#### HTTP Client + HTML Parser

- **HTTP Client**: HttpClient or RestSharp
- **HTML Parser**: AngleSharp or CsQuery

#### All-In-One Web Scraping Framework

- HtmlAgilityPack

### Dynamic Web Pages

#### All-In-One Browser Automation Framework

- Microsoft.Playwright, PuppeteerSharp, or Selenium.WebDriver

## Guides and Tutorials

### General Guides

- [Web Scraping with C# - 2024 Guide](https://brightdata.com/blog/how-tos/web-scraping-with-c-sharp)

### Proxies

- [How to Use a Proxy in C#](https://brightdata.com/blog/how-tos/proxy-with-c-sharp)

### Comparisons

- [C# vs. Python for Web Scraping Guide](https://brightdata.com/blog/how-tos/c-sharp-vs-python-for-web-scraping)
- [C# vs JavaScript for Web Scraping](https://brightdata.com/blog/web-data/c-sharp-vs-javascript)
- [Java vs C# for Web Scraping](https://brightdata.com/blog/web-data/java-vs-c-sharp)
- [C# vs. C++ for Web Scraping: Which One to Use?](https://brightdata.com/blog/web-data/c-sharp-vs-c-plus-plus-for-web-scraping)
- [Best 5 C# HTML Parsers: A Detailed Comparison Guide](https://brightdata.com/blog/web-data/best-c-sharp-html-parsers)
