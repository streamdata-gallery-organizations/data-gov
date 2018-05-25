{
  "info": {
    "name": "Data.gov API Get Datasets",
    "_postman_id": "13407c7e-533a-472a-ae39-9377568d317c",
    "description": "List or search all datasets",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "27726817-6ff6-4147-98b0-45241902bc94",
          "name": "getDatasets",
          "request": {
            "url": "http://catalog.data.gov/api/3/datasets/?badge=%7B%7D&extra=%7B%7D&facets=%7B%7D&featured=%7B%7D&format=%7B%7D&geozone=%7B%7D&granularity=%7B%7D&license=%7B%7D&organization=%7B%7D&owner=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&reuses=%7B%7D&sort=%7B%7D&tag=%7B%7D&temporal_coverage=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List or search all datasets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93c1c528-5ded-4b4e-b7c9-e02746e0ea24"
            }
          ]
        }
      ]
    }
  ]
}