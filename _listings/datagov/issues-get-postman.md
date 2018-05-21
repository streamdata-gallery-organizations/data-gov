{
  "info": {
    "name": "Data.gov API Get Issues",
    "_postman_id": "3c400c0e-4f1a-41a4-b19c-21932e6b29ee",
    "description": "List all Issues",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "issues",
      "item": [
        {
          "id": "4b2fc89f-4e79-4b31-b8b7-0c0ad22c5a7a",
          "name": "getIssues",
          "request": {
            "url": "http://catalog.data.gov/api/3/issues/?closed=%7B%7D&for=%7B%7D&page=%7B%7D&page_size=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all Issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6a9f48d-3a4a-48f6-9c4b-b7ede1a0da6f"
            }
          ]
        }
      ]
    }
  ]
}