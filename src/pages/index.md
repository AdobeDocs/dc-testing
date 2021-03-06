---
title: Overview - Adobe Analytics
description: This is the overview page of Adobe Analytics
contributors:
  - https://github.com/icaraps 
---

<Hero slots="heading, text"/> 

# EXAMPLE DOC

Adobe Product API offers limitless ways to integrate your most important customer data into key business processes. Adobe Product API offer limitless ways. xxxxx

<Resources slots="heading, links"/>

#### Resources

* [Quickstart Guide](https://www.adobe.io/apis/experiencecloud/analytics/docs.html)
* [Adobe Analytics Github Repo](https://github.com/AdobeDocs/analytics-2.0-apis)

## Ben's Test Pages

* [IO Look and feel UI](10_1_IOheaderfooter_guide/index.html)

    * [Default DC Enterprise UI](developerguide/index.html)
    * [Microsoft partnership dev doc](dcsdk_experiment/index.html)

* [IO/Adobe Look and feel API reference](doxygen_apireference/html/index.html)

    * [Current live API reference](html/index.html)
    * TBD JavaDoc (This is trivial)
    * TBD REST/Swagger  (in progress--not trivial)

## Ben's notes

* Ben is now on the XE content team under DLW. Under consideration: XE team supporting dev content onboarding to IO. 
* Zero $$ and few people hours to migrate docs to IO: process needs to be simple, fast, free. 
* We're thinking about how to support CC and DC developer content via feature rich yet simple publishing pipelines 
* Creating a product-agnostic Adobe-branded template library is relatively trivial.
* Python's Sphinx/RST pipeline offers a rich set of out of the box features. As easy as .md. Does not require contractors. Simplifies onboarding. 100% HTML5/Web support without contractors, including all industry best practice content widgets: 
   * Super fast doc level search
   * Nav: back to top, prev/next, collapsible menus, breadcrumbs
   * Sortable tables, embedded Lucichart diagrams, etc.
   * Include files, scripted integration with code for code samples, conditionalized output.
   * Internationalization possible. MT loc experiment authorized. 
   * Nearly instantaneous theme switching to change look/feel/theme.
   * Programattic PDF creation via Latex or rst2PDF (mostly facilitates content reviews via Acrobat's review feature, but also useful for downloadable guides). 

## Overview

This documentation provides instructions for Adobe Analytics 2.0 APIs. For working with Analytics 1.4 APIs, see [Analytics 1.4 API Documentation](https://github.com/AdobeDocs/analytics-1.4-apis).

The Adobe Analytics APIs are a collection of APIs that power Adobe Analytics products like Analysis Workspace. 
The APIs allow for the creation of data rich user interfaces that you can use to manipulate and integrate data.
You can also create reports to explore, get insights, or answer important questions about your data.

## Discover 

<DiscoverBlock width="100%" slots="heading, link, text"/>

### Get Started

[Quickstart Guide](guides/)
    
Get started with the Adobe Analytics APIs.

<DiscoverBlock slots="heading, link, text"/> 

### Guides

[Calculated Metrics API](guides/calculated_metrics_api/) 
     
Returns information on the user's company that is necessary for making other Adobe Analytics API calls.

<DiscoverBlock slots="link, text"/>

[Segments API](guides/segments_api/) 

Provides configuration guidance and best practices for the /segments endpoint.

<DiscoverBlock slots="link, text"/>

[Reporting Guide API](guides/reporting_api/)

Provides configuration guidance and best practices for the /reports endpoint.

<DiscoverBlock slots="link, text"/>

[Migrating from 1.4 to 2.0](guides/migrating/)

For help migrating from the 1.4 versions of the Analytics API to the newer and more capable /reports API.   

<DiscoverBlock width="100%" slots="heading, link, text"/>

### API References

[Try the API](api/) 

Try the Analytics API with Swagger UI. Explore, make calls, with full endpoint descriptions.

## Contributing 

We encourage you to participate in our open documentation initiative, if you have suggestions, corrections, additions 
or deletions for this documentation, check out the source from [this github repo](https://github.com/adobe/gatsby-theme-spectrum-example), and submit a pull 
request with your contribution. For more information, refer to the [contributing page](support/contribute/).

## API Requests & Rate Limits

The timeout for API requests through adobe.io is currently *60 seconds*.

The default rate limit for an Adobe Analytics Company is *120 requests per minute*. (The limit is enforced as *12 requests every 6 seconds*).
When rate limiting is being enforced you will get `429` HTTP response codes with the following response body: `{"error_code":"429050","message":"Too many requests"}`    