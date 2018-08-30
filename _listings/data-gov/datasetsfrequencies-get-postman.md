{
  "info": {
    "name": "Data.gov API Get Datasets Frequencies",
    "_postman_id": "f00f8eb5-a881-493f-9f4e-ddb27d5e75e3",
    "description": "List all available frequencies",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "df14d779-43c9-45e6-a32c-c693f49cb7ae",
          "name": "getDatasetsFrequencies",
          "request": {
            "url": "http://catalog.data.gov/api/3/datasets/frequencies/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all available frequencies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9213b7b5-238b-47bb-8a15-5b1cb499f9a4"
            }
          ]
        }
      ]
    }
  ]
}