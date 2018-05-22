---
swagger: "2.0"
x-collection-name: Google Search Console
x-complete: 0
info:
  title: Google Search Console API Update Site
  description: Adds a site to the set of the user's sites in Search Console.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /webmasters/v3
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