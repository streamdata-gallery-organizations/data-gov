{
  "info": {
    "name": "Data.gov API Delete Datasets  Followers",
    "_postman_id": "b5e4c891-38e9-44e5-b1d5-543fb7a5333f",
    "description": "Unfollow an object given its ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "60e0b760-f589-4957-b4d5-d2d612a1abb7",
          "name": "deleteDatasetsFollowers",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unfollow an object given its ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "958999ef-c6e2-4ffe-9c8c-5ac17bb4b9d4"
            }
          ]
        }
      ]
    }
  ]
}