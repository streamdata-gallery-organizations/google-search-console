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