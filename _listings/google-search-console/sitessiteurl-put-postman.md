{
  "info": {
    "name": "Google Search Console API Update Site",
    "_postman_id": "75e573cd-e662-497e-9083-50909d61534e",
    "description": "Adds a site to the set of the user's sites in Search Console.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Site",
      "item": [
        {
          "id": "cf89c153-08f1-45ba-a484-176efbd782b1",
          "name": "webmasters.sites.list",
          "request": {
            "url": "http://www.googleapis.com/webmasters/v3/sites",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the user's Search Console sites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b1b8955-4a69-4834-8b8a-74a5c1c4d39d"
            }
          ]
        },
        {
          "id": "bdbb8cd3-98ca-454f-a143-39168dda7dc8",
          "name": "webmasters.sites.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "webmasters",
                "v3",
                "sites/:siteUrl"
              ],
              "variable": [
                {
                  "id": "siteUrl",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about specific site."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe93f2bd-6595-4811-8617-724d56409458"
            }
          ]
        },
        {
          "id": "dd87e03e-f8d1-4cd6-b3e8-b1ade660ab54",
          "name": "webmasters.sites.add",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "webmasters",
                "v3",
                "sites/:siteUrl"
              ],
              "variable": [
                {
                  "id": "siteUrl",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a site to the set of the user's sites in Search Console."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f23ac05-f362-40ae-9a88-0c95a5912ae8"
            }
          ]
        },
        {
          "id": "4a6872b7-4a02-43d2-a730-db1338a7bd65",
          "name": "webmasters.sites.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "webmasters",
                "v3",
                "sites/:siteUrl"
              ],
              "variable": [
                {
                  "id": "siteUrl",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a site from the set of the user's Search Console sites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f40364d9-1bf2-4761-a415-c0e549383983"
            }
          ]
        }
      ]
    }
  ]
}