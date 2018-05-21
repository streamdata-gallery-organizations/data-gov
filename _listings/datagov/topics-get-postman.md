{
  "info": {
    "name": "Data.gov API Get Topics",
    "_postman_id": "0468cf74-85e4-4662-af03-bb21562cc17c",
    "description": "List all topics",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "topics",
      "item": [
        {
          "id": "06816d72-6a61-4248-89e0-3a192d6addb2",
          "name": "getTopics",
          "request": {
            "url": "http://catalog.data.gov/api/3/topics/?page=%7B%7D&page_size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all topics"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c6f7943-2cad-4100-aeba-b2a8f3d27397"
            }
          ]
        }
      ]
    }
  ]
}