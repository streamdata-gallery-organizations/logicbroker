---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Match items with CSV.
  version: 1.0.0
  description: Request rate limited to 1 request per second with bursts up to 2 requests.
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
  /api/v1/Acknowledgements/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Update acknowledgement status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_UpdateAckStatus
      x-api-path-slug: apiv1acknowledgementslogicbrokerkeystatusstatus-put
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      - in: path
        name: Status
        description: The Status
      responses:
        200:
          description: OK
      tags:
      - Acknowledgement
      - Status
  /api/v1/Acknowledgements/{LogicbrokerKey}/Status:
    get:
      summary: Retrieve acknowledgement status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Acknowledgement_GetAckStatus
      x-api-path-slug: apiv1acknowledgementslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Acknowledgement
      - Status
  /api/v1/Acknowledgements/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Acknowledgement_GetDocumentExportToken
      x-api-path-slug: apiv1acknowledgementsexport-get
      parameters:
      - in: query
        name: delimiter
        description: The column delimiter to use for CSV export
      - in: query
        name: fields
        description: The fields to export
      - in: query
        name: fileType
        description: Valid options are csv, xlsx, xml, json and legacy
      - in: query
        name: filter.advanced
        description: Advanced query options
      - in: query
        name: filter.from
        description: Beginning of time search window
      - in: query
        name: filter.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: filter.page
        description: Page number
      - in: query
        name: filter.pageSize
        description: Page size
      - in: query
        name: filter.partnerPO
        description: The partners purchase order number
      - in: query
        name: filter.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: filter.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: filter.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: filter.status
        description: The status of the document
      - in: query
        name: filter.to
        description: End of time search window
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker keys
      responses:
        200:
          description: OK
      tags:
      - Export
      - To
      - CSV
      - XLSX
  /api/v1/Acknowledgements/{LogicbrokerKey}/EDI:
    get:
      summary: Retrieve EDI
      description: Returns the latest EDI related to this document that was either
        sent or received by Logicbroker. The EDI output may also contain other documents
        that were in the same batch.
      operationId: Acknowledgement_GetDocumentEDI
      x-api-path-slug: apiv1acknowledgementslogicbrokerkeyedi-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - EDI
  /api/v1/Acknowledgements/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Acknowledgement_Import
      x-api-path-slug: apiv1acknowledgementsimport-post
      parameters:
      - in: query
        name: aliases
        description: List of field names and aliases
      - in: query
        name: custom
        description: False for standard format, true if using custom mapping configured
          by Logicbroker
      - in: query
        name: delimiter
        description: Delimiter (CSV only)
      - in: query
        name: dryRun
        description: Return shipment list instead of saving
      - in: formData
        name: file
        description: File to import
      - in: query
        name: fileType
        description: CSV or XLSX
      responses:
        200:
          description: OK
      tags:
      - Import
      - From
      - Flat
      - File
  /api/v1/ActivityEvents:
    get:
      summary: Get events for given fitlers
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_SearchActivityEvent
      x-api-path-slug: apiv1activityevents-get
      parameters:
      - in: query
        name: Filters.category
        description: Gets or sets the invoice number
      - in: query
        name: Filters.documentType
        description: Gets or sets the shipment number
      - in: query
        name: Filters.from
        description: Gets or sets the start date
      - in: query
        name: Filters.level
        description: Gets or sets the status
      - in: query
        name: Filters.linkKey
        description: Gets or sets the order number
      - in: query
        name: Filters.logicbrokerKey
        description: Gets or sets the order number
      - in: query
        name: Filters.page
        description: Gets or sets the page
      - in: query
        name: Filters.processed
        description: Gets or sets the company id
      - in: query
        name: Filters.receiverId
        description: Gets or sets the company id
      - in: query
        name: Filters.senderId
        description: Gets or sets the partner company id
      - in: query
        name: Filters.to
        description: Gets or sets the end date
      - in: query
        name: Filters.typeId
        description: Gets or sets the event type id
      - in: query
        name: Filters.viewed
        description: Gets or sets the company id
      responses:
        200:
          description: OK
      tags:
      - Eventsgiven
      - Fitlers
    post:
      summary: Create an activity event.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_CreateEvent
      x-api-path-slug: apiv1activityevents-post
      parameters:
      - in: body
        name: ActivityEvent
        description: The Activity Event
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Activity
      - Event
  /api/v1/ActivityEvents/{EventId}:
    get:
      summary: Gets the event with the specified id.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_GetActivityEvent
      x-api-path-slug: apiv1activityeventseventid-get
      parameters:
      - in: path
        name: EventId
        description: The id to search for
      responses:
        200:
          description: OK
      tags:
      - S
      - Event
      - Specified
      - Id
    put:
      summary: Update activity event
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_UpdateActivityEvent
      x-api-path-slug: apiv1activityeventseventid-put
      parameters:
      - in: body
        name: activityEvent
        description: The updated activityEvent
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: EventId
        description: The Event Id
      responses:
        200:
          description: OK
      tags:
      - Activity
      - Event
  /api/v1/ActivityEvents/EventTypes:
    get:
      summary: Gets a list of all possible event types.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: ActivityEvent_GetEventTypes
      x-api-path-slug: apiv1activityeventseventtypes-get
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - ""
      - Possible
      - Event
      - Types
  /api/v1/Attachments:
    get:
      summary: Get a list of all attachments matching a given filter.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_GetList
      x-api-path-slug: apiv1attachments-get
      parameters:
      - in: query
        name: acknowledged
        description: Acknowledged flag
      - in: query
        name: logicbrokerKey
        description: Logicbroker key
      - in: query
        name: page
        description: Page number
      - in: query
        name: receiverId
        description: Receiver account number
      - in: query
        name: type
        description: Attachment type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Attachments
      - Matching
      - Given
      - Filter
    post:
      summary: Upload an attachment
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_Upload
      x-api-path-slug: apiv1attachments-post
      parameters:
      - in: body
        name: data
        description: XML/JSON data to attach (webhooks)
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: description
        description: Attachment description
      - in: formData
        name: file
        description: File to attach
      - in: query
        name: logicbrokerKey
        description: Logicbroker key to attach
      - in: query
        name: notify
        description: If true, create an activty event
      - in: query
        name: receiverId
        description: Receiver account number
      - in: query
        name: type
        description: Attachment type (json, xml, csv, txt, pdf, png)
      - in: query
        name: url
        description: URL of file to attach
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Attachment
  /api/v1/Attachments/{container}/{name}:
    get:
      summary: Retrieve a file from Logicbroker storage.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_DownloadWithCoId
      x-api-path-slug: apiv1attachmentscontainername-get
      parameters:
      - in: path
        name: container
        description: File container (ex
      - in: path
        name: name
        description: File name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - File
      - From
      - Logicbroker
      - Storage
  /api/v1/Document/Script/{ScriptName}:
    get:
      summary: Execute custom handler.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Document_GetCustomScript
      x-api-path-slug: apiv1documentscriptscriptname-get
      parameters:
      - in: path
        name: ScriptName
        description: The custom script name
      responses:
        200:
          description: OK
      tags:
      - Execute
      - Custom
      - Handler
    post:
      summary: Execute custom handler.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Document_PostCustomScript
      x-api-path-slug: apiv1documentscriptscriptname-post
      parameters:
      - in: path
        name: ScriptName
        description: The custom script name
      responses:
        200:
          description: OK
      tags:
      - Execute
      - Custom
      - Handler
    options:
      summary: Execute custom handler.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Document_OptionsCustomScript
      x-api-path-slug: apiv1documentscriptscriptname-options
      parameters:
      - in: path
        name: ScriptName
        description: The custom script name
      responses:
        200:
          description: OK
      tags:
      - Execute
      - Custom
      - Handler
  /api/v1/Inventory/{partnerId}:
    get:
      summary: Download inventory as CSV.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Inventory_Download
      x-api-path-slug: apiv1inventorypartnerid-get
      parameters:
      - in: query
        name: fileType
        description: CSV or XLSX
      - in: query
        name: includeNullQuantity
        description: Set to true to include items with null quantity
      - in: query
        name: mapped
        description: Set to false to view items with no merchant SKU
      - in: query
        name: modifiedAfter
        description: Only items modified after this time
      - in: path
        name: partnerId
        description: Partner account number
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Download
      - Inventory
      - As
      - CSV
    post:
      summary: Import inventory from CSV.
      description: Request rate limited to 1 request per second with bursts up to
        2 requests.
      operationId: Inventory_Upload
      x-api-path-slug: apiv1inventorypartnerid-post
      parameters:
      - in: formData
        name: file
        description: File to import
      - in: path
        name: partnerId
        description: Partner account number
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Import
      - Inventory
      - From
      - CSV
    delete:
      summary: Delete all inventory records.
      description: Request rate limited to 1 request every 60 seconds with bursts
        up to 2 requests.
      operationId: Inventory_DeleteAll
      x-api-path-slug: apiv1inventorypartnerid-delete
      parameters:
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Inventory
      - Records
  /api/v1/Inventory/Broadcast:
    post:
      summary: Import inventory from CSV.
      description: Request rate limited to 1 request every 60 seconds with bursts
        up to 2 requests.
      operationId: Inventory_Broadcast
      x-api-path-slug: apiv1inventorybroadcast-post
      parameters:
      - in: formData
        name: file
        description: File to import
      - in: query
        name: transform
        description: Transform CSV (if configured)
      responses:
        200:
          description: OK
      tags:
      - Import
      - Inventory
      - From
      - CSV
  /api/v1/Inventory/{partnerId}/Matching:
    post:
      summary: Match items with CSV.
      description: Request rate limited to 1 request per second with bursts up to
        2 requests.
      operationId: Inventory_UploadMatching
      x-api-path-slug: apiv1inventorypartneridmatching-post
      parameters:
      - in: formData
        name: file
        description: File to import
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Match
      - Items
      - CSV
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