---
swagger: "2.0"
x-collection-name: Google Search Console
x-complete: 0
info:
  title: Google URL Testing Tools API Run Mobile Friendly Test
  description: Runs Mobile-Friendly Test for a given URL.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: searchconsole.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sites:
    get:
      summary: Get Sites
      description: Lists the user's Search Console sites.
      operationId: webmasters.sites.list
      x-api-path-slug: sites-get
      responses:
        200:
          description: OK
      tags:
      - Site
  /sites/{siteUrl}:
    delete:
      summary: Remove Site
      description: Removes a site from the set of the user's Search Console sites.
      operationId: webmasters.sites.delete
      x-api-path-slug: sitessiteurl-delete
      parameters:
      - in: path
        name: siteUrl
        description: The URI of the property as defined in Search Console
      responses:
        200:
          description: OK
      tags:
      - Site
    get:
      summary: Get Site
      description: Retrieves information about specific site.
      operationId: webmasters.sites.get
      x-api-path-slug: sitessiteurl-get
      parameters:
      - in: path
        name: siteUrl
        description: The URI of the property as defined in Search Console
      responses:
        200:
          description: OK
      tags:
      - Site
    put:
      summary: Update Site
      description: Adds a site to the set of the user's sites in Search Console.
      operationId: webmasters.sites.add
      x-api-path-slug: sitessiteurl-put
      parameters:
      - in: path
        name: siteUrl
        description: The URL of the site to add
      responses:
        200:
          description: OK
      tags:
      - Site
  /sites/{siteUrl}/searchAnalytics/query:
    post:
      summary: Query Data
      description: |-
        Query your data with filters and parameters that you define. Returns zero or more rows grouped by the row keys that you define. You must define a date range of one or more days.

        When date is one of the group by values, any days without data are omitted from the result list. If you need to know which days have data, issue a broad date range query grouped by date for any metric, and see which day rows are returned.
      operationId: webmasters.searchanalytics.query
      x-api-path-slug: sitessiteurlsearchanalyticsquery-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Data
  /sites/{siteUrl}/sitemaps:
    get:
      summary: List Sitemap
      description: Lists the sitemaps-entries submitted for this site, or included
        in the sitemap index file (if sitemapIndex is specified in the request).
      operationId: webmasters.sitemaps.list
      x-api-path-slug: sitessiteurlsitemaps-get
      parameters:
      - in: query
        name: sitemapIndex
        description: A URL of a sites sitemap index
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Sitemap
  /sites/{siteUrl}/sitemaps/{feedpath}:
    delete:
      summary: Delete Sitemap
      description: Deletes a sitemap from this site.
      operationId: webmasters.sitemaps.delete
      x-api-path-slug: sitessiteurlsitemapsfeedpath-delete
      parameters:
      - in: path
        name: feedpath
        description: The URL of the actual sitemap
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Sitemap
    get:
      summary: Get Sitemap
      description: Retrieves information about a specific sitemap.
      operationId: webmasters.sitemaps.get
      x-api-path-slug: sitessiteurlsitemapsfeedpath-get
      parameters:
      - in: path
        name: feedpath
        description: The URL of the actual sitemap
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Sitemap
    put:
      summary: Update Sitemap
      description: Submits a sitemap for a site.
      operationId: webmasters.sitemaps.submit
      x-api-path-slug: sitessiteurlsitemapsfeedpath-put
      parameters:
      - in: path
        name: feedpath
        description: The URL of the sitemap to add
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Sitemap
  /sites/{siteUrl}/urlCrawlErrorsCounts/query:
    get:
      summary: Get Crawl Error Count
      description: Retrieves a time series of the number of URL crawl errors per error
        category and platform.
      operationId: webmasters.urlcrawlerrorscounts.query
      x-api-path-slug: sitessiteurlurlcrawlerrorscountsquery-get
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: latestCountsOnly
        description: If true, returns only the latest crawl error counts
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Error
  /sites/{siteUrl}/urlCrawlErrorsSamples:
    get:
      summary: Get Crawl Error Samples
      description: Lists a site's sample URLs for the specified crawl error category
        and platform.
      operationId: webmasters.urlcrawlerrorssamples.list
      x-api-path-slug: sitessiteurlurlcrawlerrorssamples-get
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - Error
  /sites/{siteUrl}/urlCrawlErrorsSamples/{url}:
    delete:
      summary: Delete Crawl Error Samples
      description: Marks the provided site's sample URL as fixed, and removes it from
        the samples list.
      operationId: webmasters.urlcrawlerrorssamples.markAsFixed
      x-api-path-slug: sitessiteurlurlcrawlerrorssamplesurl-delete
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      - in: path
        name: url
        description: The relative path (without the site) of the sample URL
      responses:
        200:
          description: OK
      tags:
      - Error
    get:
      summary: Get Crawl Error Sample
      description: Retrieves details about crawl errors for a site's sample URL.
      operationId: webmasters.urlcrawlerrorssamples.get
      x-api-path-slug: sitessiteurlurlcrawlerrorssamplesurl-get
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The sites URL, including protocol
      - in: path
        name: url
        description: The relative path (without the site) of the sample URL
      responses:
        200:
          description: OK
      tags:
      - Error
  /v1/urlTestingTools/mobileFriendlyTest:run:
    post:
      summary: Run Mobile Friendly Test
      description: Runs Mobile-Friendly Test for a given URL.
      operationId: searchconsole.urlTestingTools.mobileFriendlyTest.run
      x-api-path-slug: v1urltestingtoolsmobilefriendlytestrun-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Test
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---