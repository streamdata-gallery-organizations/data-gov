{
  "info": {
    "name": "Data.gov API Get Datasets Checkurl",
    "_postman_id": "e05bed52-1866-4902-9bbb-473e724163ab",
    "description": "Checks that a URL exists and returns metadata",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "84a9b1a8-fb5f-46d5-886e-b96c42738001",
          "name": "getDatasetsCheckurl",
          "request": {
            "url": "http://catalog.data.gov/api/3/datasets/checkurl/?group=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks that a URL exists and returns metadata"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20e10b7f-f34f-4798-9fa4-bd1617b687e8"
            }
          ]
        }
      ]
    }
  ]
}