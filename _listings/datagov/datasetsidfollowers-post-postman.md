{
  "info": {
    "name": "Data.gov API Add Datasets  Followers",
    "_postman_id": "67d9f96b-1629-4866-8407-7917db05e105",
    "description": "Follow an object given its ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "1466296b-a291-4053-addf-2c9bb263d301",
          "name": "postDatasetsFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:id/followers/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Follow an object given its ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a199f24-eca4-47d2-8662-ecc992e20d7b"
            }
          ]
        }
      ]
    }
  ]
}