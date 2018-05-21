{
  "info": {
    "name": "Data.gov API Delete Datasets Dataset",
    "_postman_id": "f2294af4-d5c3-494a-8f34-c6e3cf277510",
    "description": "Delete a dataset given its identifier",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "datasets",
      "item": [
        {
          "id": "a0611fe7-9931-490e-8c93-c88d0d68564a",
          "name": "deleteDatasetsDataset",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a dataset given its identifier"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee64b896-87d0-4295-97e4-287e5089079d"
            }
          ]
        }
      ]
    }
  ]
}