{
  "info": {
    "name": "Logic Broker CommerceAPI Execute custom handler.",
    "_postman_id": "301f8151-ef6b-4a17-ac11-26704e2e4c83",
    "description": "Request rate limited to 2 requests per second with bursts up to 25 requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Execute",
      "item": [
        {
          "id": "2a2dfba4-97a3-4904-b506-103795529b8d",
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
              "id": "0ea6a26d-6cb9-46c7-88b7-8234c4bd6756"
            }
          ]
        },
        {
          "id": "486961f9-9fce-41fc-9b2c-ab18573b3231",
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
              "id": "3ca04eb3-e38b-4d4d-a652-8ad8ad65444d"
            }
          ]
        }
      ]
    }
  ]
}