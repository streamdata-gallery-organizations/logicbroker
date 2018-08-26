{
  "info": {
    "name": "Logic Broker CommerceAPI Execute custom handler.",
    "_postman_id": "7199cd34-52cd-4262-a60c-e4f0d1943e8d",
    "description": "Request rate limited to 2 requests per second with bursts up to 25 requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Execute",
      "item": [
        {
          "id": "986df464-ffb4-4692-8934-4fa7d40bc17f",
          "name": "Document_GetCustomScript",
          "request": {
            "url": {
              "protocol": "http",
              "host": "stage.commerceapi.io",
              "path": [
                "api/v1/Document/Script/:ScriptName"
              ],
              "variable": [
                {
                  "id": "ScriptName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Request rate limited to 2 requests per second with bursts up to 25 requests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ab2d6f9-50a5-4caa-be4c-95eefb77bdd0"
            }
          ]
        }
      ]
    }
  ]
}