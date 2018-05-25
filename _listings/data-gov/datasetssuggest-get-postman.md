{
  "info": {
    "name": "Data.gov API Get Datasets Suggest",
    "_postman_id": "26d2447c-7cae-4b71-88d7-b0f8ed9c6710",
    "description": "Suggest datasets",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "bed7f9d3-6de2-4e0e-8e04-91f8203ee954",
          "name": "getDatasetsSuggest",
          "request": {
            "url": "http://catalog.data.gov/api/3/datasets/suggest/?q=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Suggest datasets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "619825cf-b35d-4bc8-9696-8057892f8c09"
            }
          ]
        }
      ]
    }
  ]
}