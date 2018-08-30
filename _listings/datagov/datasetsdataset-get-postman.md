{
  "info": {
    "name": "Data.gov API Get Datasets Dataset",
    "_postman_id": "0d04cf48-714d-408e-9831-511c1d183b34",
    "description": "Get a dataset given its identifier",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "bbfcf709-0b5a-40ff-a611-327f09e3f08f",
          "name": "getDatasetsDataset",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "datasets/:dataset/"
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
              "id": "d7ab0356-cdeb-42f5-b757-c96297ffeee3"
            }
          ]
        }
      ]
    }
  ]
}