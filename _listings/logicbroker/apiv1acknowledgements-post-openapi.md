---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Create an acknowledgement
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Acknowledgements/{LogicbrokerKey}:
    get:
      summary: Get acknowledgement details
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_GetAck
      x-api-path-slug: apiv1acknowledgementslogicbrokerkey-get
      parameters:
      - in: path
        name: LogicbrokerKey
      responses:
        200:
          description: OK
      tags:
      - Acknowledgement
      - Details
  /api/v1/Acknowledgements/CustomXML:
    post:
      summary: Create acknowledgement(s) based on custom XML.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_UploadCustomXml
      x-api-path-slug: apiv1acknowledgementscustomxml-post
      parameters:
      - in: body
        name: data
        description: XML data to upload
        schema:
          $ref: '#/definitions/holder'
      - in: formData
        name: file
        description: File to upload
      - in: query
        name: xmlType
        description: XML type, leave blank unless directed otherwise
      responses:
        200:
          description: OK
      tags:
      - Acknowledgement(s)
      - Based
      - "On"
      - Custom
      - XML
  /api/v1/Acknowledgements/Request:
    post:
      summary: Request an acknowledgement from a trading partner
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_RequestAck
      x-api-path-slug: apiv1acknowledgementsrequest-post
      parameters:
      - in: body
        name: Acknowledgement
        description: Acknowledgement request object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Acknowledgement
      - From
      - Trading
      - Partner
  /api/v1/Acknowledgements:
    get:
      summary: Search acknowledgements
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_SearchAcks
      x-api-path-slug: apiv1acknowledgements-get
      parameters:
      - in: query
        name: filters.advanced
        description: Advanced query options
      - in: query
        name: filters.from
        description: Beginning of time search window
      - in: query
        name: filters.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: filters.page
        description: Page number
      - in: query
        name: filters.pageSize
        description: Page size
      - in: query
        name: filters.partnerPO
        description: The partners purchase order number
      - in: query
        name: filters.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: filters.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: filters.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: filters.status
        description: The status of the document
      - in: query
        name: filters.to
        description: End of time search window
      responses:
        200:
          description: OK
      tags:
      - Search
      - Acknowledgements
    post:
      summary: Create an acknowledgement
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_CreateAck
      x-api-path-slug: apiv1acknowledgements-post
      parameters:
      - in: body
        name: Acknowledgement
        description: Acknowledgement object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Acknowledgement
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---