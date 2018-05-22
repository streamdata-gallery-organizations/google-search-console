{
  "info": {
    "name": "Google Search Console API Get Sites",
    "_postman_id": "d4d0f6ac-57f0-4d98-83ed-779ac5b16477",
    "description": "Lists the user's Search Console sites.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Site",
      "item": [
        {
          "id": "1ccec76f-7139-4159-82f0-f401a589206c",
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
              "id": "d37bed0b-0274-4155-a555-f17c1f6abbec"
            }
          ]
        }
      ]
    }
  ]
}