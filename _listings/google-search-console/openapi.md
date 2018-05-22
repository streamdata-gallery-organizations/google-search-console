---
swagger: "2.0"
x-collection-name: Google Search Console
x-complete: 1
info:
  title: Google Search Console URL Testing Tools
  description: provides-tools-for-running-validation-tests-against-single-urls
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
---