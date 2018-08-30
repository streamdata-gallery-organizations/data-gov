{
  "info": {
    "name": "Data.gov API Get Issues",
    "_postman_id": "5fc5bc12-484c-4fda-9965-d2a0d0de9ea5",
    "description": "Get an issue given its ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "issues",
      "item": [
        {
          "id": "56edf50a-ba44-46f7-b730-0fb31d04ceec",
          "name": "getIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "issues/:id/"
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
            "description": "Get an issue given its ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0b1312c-e3d8-4341-98b4-5b1bb6894078"
            }
          ]
        }
      ]
    }
  ]
}