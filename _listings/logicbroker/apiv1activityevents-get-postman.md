{
  "info": {
    "name": "Logic Broker CommerceAPI Get events for given fitlers",
    "_postman_id": "2581719f-5870-433f-b42c-27857c854ebc",
    "description": "Request rate limited to 10 requests per second with bursts up to 100 requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Eventsgiven",
      "item": [
        {
          "id": "9ddc6bd9-7c8c-4539-9e24-a696c188acf1",
          "name": "ActivityEvent_SearchActivityEvent",
          "request": {
            "url": "http://stage.commerceapi.io/api/v1/ActivityEvents?Filters.category=%7B%7D&Filters.documentType=%7B%7D&Filters.from=%7B%7D&Filters.level=%7B%7D&Filters.linkKey=%7B%7D&Filters.logicbrokerKey=%7B%7D&Filters.page=%7B%7D&Filters.processed=%7B%7D&Filters.receiverId=%7B%7D&Filters.senderId=%7B%7D&Filters.to=%7B%7D&Filters.typeId=%7B%7D&Filters.viewed=%7B%7D",
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
              "id": "463eb50d-33c1-42b1-9d6a-654e835e3c7c"
            }
          ]
        }
      ]
    }
  ]
}