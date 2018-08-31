{
  "info": {
    "name": "Google Search Console API Get Site",
    "_postman_id": "f478067c-e15f-49e2-824f-0633facf1bbc",
    "description": "Retrieves information about specific site.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Site",
      "item": [
        {
          "id": "0317b731-4fde-44ff-8e49-23df5dc5a4da",
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
              "id": "198b43e6-fe57-4834-8e74-b13365d15e46"
            }
          ]
        },
        {
          "id": "ef4e86c9-9eea-4de4-8f29-e347527d353f",
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
              "id": "0d4739d7-f724-436a-8deb-50692515866c"
            }
          ]
        },
        {
          "id": "aa30b894-a1da-4fa0-b083-169881f3fe32",
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
              "id": "454559a1-4497-4964-8b6c-159df08f5e3e"
            }
          ]
        }
      ]
    }
  ]
}