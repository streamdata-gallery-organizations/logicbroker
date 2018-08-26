{
  "info": {
    "name": "Logic Broker CommerceAPI Execute custom handler.",
    "_postman_id": "a8aa40b9-080e-4b00-b1bc-9d6c680edb01",
    "description": "Request rate limited to 2 requests per second with bursts up to 25 requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Execute",
      "item": [
        {
          "id": "a3e29fce-18ee-4633-a109-07ccddeea4c2",
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
              "id": "2a623b17-9353-4f23-8ba5-b678be487740"
            }
          ]
        },
        {
          "id": "1f8d1dcd-8acb-471a-90f8-9599f199f053",
          "name": "Document_PostCustomScript",
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
            "method": "POST",
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
              "id": "bb6c0449-ec5d-4aa7-b364-5c02e46cace3"
            }
          ]
        }
      ]
    }
  ]
}