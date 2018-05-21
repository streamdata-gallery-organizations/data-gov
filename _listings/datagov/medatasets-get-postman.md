{
  "info": {
    "name": "Data.gov API Get Me Datasets",
    "_postman_id": "1b894355-61f0-4a55-8938-28758604b889",
    "description": "List all my datasets (including private ones)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "me",
      "item": [
        {
          "id": "4ee38c07-368a-4842-9d27-f6a5d1aac25f",
          "name": "getMeDatasets",
          "request": {
            "url": "http://catalog.data.gov/api/3/me/datasets/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all my datasets (including private ones)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48ac0b27-1e91-4446-b17e-631af445c368"
            }
          ]
        }
      ]
    }
  ]
}