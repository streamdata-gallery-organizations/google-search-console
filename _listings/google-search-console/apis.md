---
name: Google Search Console
x-slug: google-search-console
description: Search Console is a free service that enables you to monitor your sites
  performance in Google Search, to ensure that Google can crawl your site or app correctly,
  and to test the validity and performance of a given page. Search Console provides
  programmatic access to the service through the APIs documented here.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
x-kinRank: "9"
x-alexaRank: ""
tags: Google Search Console
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/apis.md
specificationVersion: "0.14"
apis:
- name: Google Search Console API Get Sites
  x-api-slug: google-search-console-api
  description: Lists the user's Search Console sites.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites
  tags: Site
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sites-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sites-get-openapi.md
- name: Google Search Console API Remove Site
  x-api-slug: google-search-console-api
  description: Removes a site from the set of the user's Search Console sites.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}
  tags: Site
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurl-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurl-delete-openapi.md
- name: Google Search Console API Get Site
  x-api-slug: google-search-console-api
  description: Retrieves information about specific site.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}
  tags: Site
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurl-get-openapi.md
- name: Google Search Console API Update Site
  x-api-slug: google-search-console-api
  description: Adds a site to the set of the user's sites in Search Console.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}
  tags: Site
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurl-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurl-put-openapi.md
- name: Google Search Console API Query Data
  x-api-slug: google-search-console-api
  description: |-
    Query your data with filters and parameters that you define. Returns zero or more rows grouped by the row keys that you define. You must define a date range of one or more days.

    When date is one of the group by values, any days without data are omitted from the result list. If you need to know which days have data, issue a broad date range query grouped by date for any metric, and see which day rows are returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/searchAnalytics/query
  tags: Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlsearchanalyticsquery-post-openapi.md
- name: Google Search Console API List Sitemap
  x-api-slug: google-search-console-api
  description: Lists the sitemaps-entries submitted for this site, or included in
    the sitemap index file (if sitemapIndex is specified in the request).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/sitemaps
  tags: Sitemap
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlsitemaps-get-openapi.md
- name: Google Search Console API Delete Sitemap
  x-api-slug: google-search-console-api
  description: Deletes a sitemap from this site.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/sitemaps/{feedpath}
  tags: Sitemap
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlsitemapsfeedpath-delete-openapi.md
- name: Google Search Console API Get Sitemap
  x-api-slug: google-search-console-api
  description: Retrieves information about a specific sitemap.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/sitemaps/{feedpath}
  tags: Sitemap
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlsitemapsfeedpath-get-openapi.md
- name: Google Search Console API Update Sitemap
  x-api-slug: google-search-console-api
  description: Submits a sitemap for a site.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/sitemaps/{feedpath}
  tags: Sitemap
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlsitemapsfeedpath-put-openapi.md
- name: Google Search Console API Get Crawl Error Count
  x-api-slug: google-search-console-api
  description: Retrieves a time series of the number of URL crawl errors per error
    category and platform.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/urlCrawlErrorsCounts/query
  tags: Error
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlurlcrawlerrorscountsquery-get-openapi.md
- name: Google Search Console API Get Crawl Error Samples
  x-api-slug: google-search-console-api
  description: Lists a site's sample URLs for the specified crawl error category and
    platform.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/urlCrawlErrorsSamples
  tags: Error
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlurlcrawlerrorssamples-get-openapi.md
- name: Google Search Console API Delete Crawl Error Samples
  x-api-slug: google-search-console-api
  description: Marks the provided site's sample URL as fixed, and removes it from
    the samples list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/urlCrawlErrorsSamples/{url}
  tags: Error
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlurlcrawlerrorssamplesurl-delete-openapi.md
- name: Google Search Console API Get Crawl Error Sample
  x-api-slug: google-search-console-api
  description: Retrieves details about crawl errors for a site's sample URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3//sites/{siteUrl}/urlCrawlErrorsSamples/{url}
  tags: Error
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/sitessiteurlurlcrawlerrorssamplesurl-get-openapi.md
- name: Google Search Console API
  x-api-slug: google-search-console-api
  description: Query search analytics, list your verified sites, manage your sitemaps,
    and view crawl errors for your site.The Search Console API provides programmatic
    access to most of the functionality ofGoogle Search Console. You can use the API
    to view, add, or remove properties and sitemaps, and run advanced queries for
    Google Search results data for the properties that you manage in Search Console.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://www.googleapis.com//webmasters/v3
  tags: Google Search Console
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/openapi.md
- name: Google URL Testing Tools API Run Mobile Friendly Test
  x-api-slug: google-url-testing-tools-api
  description: Runs Mobile-Friendly Test for a given URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://searchconsole.googleapis.com////v1/urlTestingTools/mobileFriendlyTest:run
  tags: Test
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/v1urltestingtoolsmobilefriendlytestrun-post-openapi.md
- name: Google URL Testing Tools API
  x-api-slug: google-url-testing-tools-api
  description: The Search Console URL Testing Tools API enables you to run various
    performance and validation checks against a single web page. These tests run as
    a non-logged-in user, with permissions of the Googlebot crawler; this means that
    if your page isrobotedto prevent access by Googlebot, these tests will not work.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/subdomains-google-webmaster-tools-13960.gif
  humanURL: https://developers.google.com/webmaster-tools/
  baseURL: ://searchconsole.googleapis.com//
  tags: Google Search Console
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-search-console/master/_listings/google-search-console/openapi.md
x-common:
- type: x-blog
  url: https://support.google.com/webmasters/go/blog
- type: x-blog-rss
  url: https://webmasters.googleblog.com/feeds/posts/default?alt=rss
- type: x-forum
  url: https://productforums.google.com/forum/#!forum/webmasters
- type: x-website
  url: https://developers.google.com/webmaster-tools/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---