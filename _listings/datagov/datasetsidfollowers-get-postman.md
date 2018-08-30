{
  "info": {
    "name": "Data.gov API Get Datasets  Followers",
    "_postman_id": "d59eb8de-a7e2-47e7-bac6-cd01e14d219f",
    "description": "List all followers for a given object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "17a8eced-015f-4b8c-9a69-8c1c08544273",
          "name": "getDatasetsFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:id/followers/"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all followers for a given object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00b313df-5bb0-44fd-9933-7d9fd6a698f5"
            }
          ]
        }
      ]
    }
  ]
}