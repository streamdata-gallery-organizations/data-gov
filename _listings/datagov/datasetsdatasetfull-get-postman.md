{
  "info": {
    "name": "Data.gov API Get Datasets Dataset Full",
    "_postman_id": "86a4f281-603b-4570-88ed-5d06b2f3e39e",
    "description": "Get a dataset given its identifier",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "604d525a-3763-4b45-bcdc-464ece270b8a",
          "name": "getDatasetsDatasetFull",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:dataset/full/"
              ],
              "variable": [
                {
                  "id": "dataset",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a dataset given its identifier"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d07009f4-bcd4-41fc-b869-b59e447d2bfd"
            }
          ]
        }
      ]
    }
  ]
}