{
  "info": {
    "name": "Google Search Console API Remove Site",
    "_postman_id": "df903cd4-c4af-4748-bb57-278a41900034",
    "description": "Removes a site from the set of the user's Search Console sites.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Site",
      "item": [
        {
          "id": "db46a1a2-0257-4f8d-b58f-24152fd97b1f",
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
              "id": "7299dc37-f718-4553-ae47-84e0e7023cbd"
            }
          ]
        },
        {
          "id": "5ea62e31-dbd0-44e6-8aab-bdfa73ca4360",
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
              "id": "32f942d7-9ac9-4371-8823-55cd0d313846"
            }
          ]
        }
      ]
    }
  ]
}