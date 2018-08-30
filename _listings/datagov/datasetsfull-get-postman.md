{
  "info": {
    "name": "Data.gov API Get Datasets Full",
    "_postman_id": "84f22eae-bde6-4e43-b491-9169cc96a5d7",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "3350215b-4192-4aea-8f9d-5db61e1f286a",
          "name": "getDatasetsFull",
          "request": {
            "url": "http://catalog.data.gov/api/3/datasets/full/?badge=%7B%7D&extra=%7B%7D&facets=%7B%7D&featured=%7B%7D&format=%7B%7D&geozone=%7B%7D&granularity=%7B%7D&license=%7B%7D&organization=%7B%7D&owner=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&reuses=%7B%7D&sort=%7B%7D&tag=%7B%7D&temporal_coverage=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Datasets Full"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c75954c-ec47-42c7-a78c-0c968d92ef55"
            }
          ]
        }
      ]
    }
  ]
}