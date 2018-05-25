{
  "info": {
    "name": "Data.gov API Get Datasets Suggest Formats",
    "_postman_id": "3dcaf0a3-b051-461f-8f8b-31ff39346c58",
    "description": "Suggest file formats",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "bba35db5-dea4-4be3-bbed-52867e96327d",
          "name": "getDatasetsSuggestFormats",
          "request": {
            "url": "http://catalog.data.gov/api/3/datasets/suggest/formats/?q=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Suggest file formats"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4753d4ba-200b-40c0-966b-f9b80d315748"
            }
          ]
        }
      ]
    }
  ]
}