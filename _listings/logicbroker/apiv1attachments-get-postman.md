{
  "info": {
    "name": "Logic Broker CommerceAPI Get a list of all attachments matching a given filter.",
    "_postman_id": "a1962b83-05f5-491d-8c9d-ac10f2b734ca",
    "description": "Request rate limited to 10 requests per second with bursts up to 100 requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "6824d3a8-cc4a-4419-a6e5-626e14e33885",
          "name": "Attachment_GetList",
          "request": {
            "url": "http://stage.commerceapi.io/api/v1/Attachments?acknowledged=%7B%7D&logicbrokerKey=%7B%7D&page=%7B%7D&receiverId=%7B%7D&type=%7B%7D",
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
              "id": "d4acf39f-9f60-45af-904e-8797197e5449"
            }
          ]
        }
      ]
    }
  ]
}