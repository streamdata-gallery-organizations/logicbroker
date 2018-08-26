{
  "info": {
    "name": "Logic Broker CommerceAPI Get acknowledgement details",
    "_postman_id": "55a6ff33-3630-496d-9466-5f41ef3cd090",
    "description": "Request rate limited to 10 requests per second with bursts up to 100 requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledgement",
      "item": [
        {
          "id": "2beb6c87-2822-4f0f-933b-f71dd5be3cea",
          "name": "Acknowledgement_GetAck",
          "request": {
            "url": {
              "protocol": "http",
              "host": "stage.commerceapi.io",
              "path": [
                "api/v1/Acknowledgements/:LogicbrokerKey"
              ],
              "variable": [
                {
                  "id": "LogicbrokerKey",
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
            "description": "Request rate limited to 10 requests per second with bursts up to 100 requests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4284b249-7569-4ba7-aeb4-3775aed22c10"
            }
          ]
        }
      ]
    }
  ]
}