---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Get shipping labels for multiple shipments
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
    delete:
      summary: Delete all SKU mappings.
      description: Request rate limited to 1 request every 60 seconds with bursts
        up to 2 requests.
      operationId: Inventory_DeleteMappings
      x-api-path-slug: apiv1inventorypartneridmatching-delete
      parameters:
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - SKU
      - Mappings
  /api/v1/Inventory/{partnerId}/Resend:
    put:
      summary: Resend all inventory items.
      description: Request rate limited to 1 request every 5 minutes with bursts up
        to 2 requests.
      operationId: Inventory_ResendAll
      x-api-path-slug: apiv1inventorypartneridresend-put
      parameters:
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Resend
      - ""
      - Inventory
      - Items
  /api/v1/Inventory/{partnerId}/Item/{sku}:
    get:
      summary: Get a single item by SKU
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Inventory_GetItem
      x-api-path-slug: apiv1inventorypartneriditemsku-get
      parameters:
      - in: path
        name: partnerId
        description: Partner account number
      - in: path
        name: sku
        description: Item SKU
      responses:
        200:
          description: OK
      tags:
      - Single
      - Item
      - By
      - SKU
  /api/v1/Inventory/Availability/{sku}:
    get:
      summary: Get the availability of an item across all suppliers.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Inventory_GetAvailability
      x-api-path-slug: apiv1inventoryavailabilitysku-get
      parameters:
      - in: path
        name: sku
        description: Merchant SKU
      responses:
        200:
          description: OK
      tags:
      - Availability
      - Of
      - Item
      - Across
      - ""
      - Suppliers
  /api/v1/Invoices/CustomXML:
    post:
      summary: Create invoice(s) based on custom XML.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_UploadCustomXml
      x-api-path-slug: apiv1invoicescustomxml-post
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
      - Invoice(s)
      - Based
      - "On"
      - Custom
      - XML
  /api/v1/Invoices:
    get:
      summary: Get invoices based on provided filters
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_SearchInvoice
      x-api-path-slug: apiv1invoices-get
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
      - Invoices
      - Based
      - "On"
      - Provided
      - Filters
    post:
      summary: Create a new invoice
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_CreateInvoice
      x-api-path-slug: apiv1invoices-post
      parameters:
      - in: body
        name: invoice
        description: The invoice to save
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Invoice
  /api/v1/Invoices/{LogicbrokerKey}/Events:
    get:
      summary: Retrieve related events
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_GetActivityEvent
      x-api-path-slug: apiv1invoiceslogicbrokerkeyevents-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Related
      - Events
  /api/v1/Invoices/{LogicbrokerKey}/EDI:
    get:
      summary: Retrieve EDI
      description: Returns the latest EDI related to this document that was either
        sent or received by Logicbroker. The EDI output may also contain other documents
        that were in the same batch.
      operationId: Invoice_GetDocumentEDI
      x-api-path-slug: apiv1invoiceslogicbrokerkeyedi-get
      parameters:
      - in: path
        name: LogicbrokerKey
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - EDI
  /api/v1/Invoices/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Invoice_Import
      x-api-path-slug: apiv1invoicesimport-post
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
        description: Return invoice list instead of saving
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
  /api/v1/Invoices/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Invoice_GetDocumentExportToken
      x-api-path-slug: apiv1invoicesexport-get
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
  /api/v1/Invoices/{LogicbrokerKey}:
    get:
      summary: Returns the invoice with the specified key.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_GetInvoice
      x-api-path-slug: apiv1invoiceslogicbrokerkey-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The logicbroker key to search for
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Invoice
      - Specified
      - Key
  /api/v1/Invoices/{LogicbrokerKey}/Status:
    get:
      summary: Return the current status code of an invoice.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_GetInvoiceStatus
      x-api-path-slug: apiv1invoiceslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The logicbroker key of the invoice to look up
      responses:
        200:
          description: OK
      tags:
      - Return
      - Current
      - Status
      - Code
      - Of
      - Invoice
  /api/v1/Invoices/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Updates an invoice to the specified status.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Invoice_UpdateInvoiceStatus
      x-api-path-slug: apiv1invoiceslogicbrokerkeystatusstatus-put
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The logicbroker key of the invoice to update
      - in: path
        name: Status
        description: The Status
      responses:
        200:
          description: OK
      tags:
      - S
      - Invoice
      - To
      - Specified
      - Status
  /api/v1/Orders/{LogicbrokerKey}/Invoices:
    get:
      summary: Retrieve a list of invoices for an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetInvoice
      x-api-path-slug: apiv1orderslogicbrokerkeyinvoices-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Invoicesan
      - Order
    post:
      summary: Creates invoice and links with the given order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_CreateInvoiceForSalesOrder
      x-api-path-slug: apiv1orderslogicbrokerkeyinvoices-post
      parameters:
      - in: body
        name: Invoice
        description: The invoice
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Invoice
      - Links
      - Given
      - Order
  /api/v1/Orders/CustomXML:
    post:
      summary: Create order(s) based on custom XML.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_UploadCustomXml
      x-api-path-slug: apiv1orderscustomxml-post
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
      - Order(s)
      - Based
      - "On"
      - Custom
      - XML
  /api/v1/Orders:
    get:
      summary: Search orders
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_SearchSalesOrders
      x-api-path-slug: apiv1orders-get
      parameters:
      - in: query
        name: Filters.advanced
        description: Advanced query options
      - in: query
        name: Filters.from
        description: Beginning of time search window
      - in: query
        name: Filters.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: Filters.page
        description: Page number
      - in: query
        name: Filters.pageSize
        description: Page size
      - in: query
        name: Filters.partnerPO
        description: The partners purchase order number
      - in: query
        name: Filters.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: Filters.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: Filters.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: Filters.status
        description: The status of the document
      - in: query
        name: Filters.to
        description: End of time search window
      responses:
        200:
          description: OK
      tags:
      - Search
      - Orders
    post:
      summary: Create an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_CreateSalesOrder
      x-api-path-slug: apiv1orders-post
      parameters:
      - in: body
        name: SalesOrder
        description: Order object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
  /api/v1/Orders/{LogicbrokerKey}/Shipments:
    get:
      summary: Retrieve a list of shipments for an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetASN
      x-api-path-slug: apiv1orderslogicbrokerkeyshipments-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Shipmentsan
      - Order
    post:
      summary: The create shipment for sales order.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_CreateShipmentForSalesOrder
      x-api-path-slug: apiv1orderslogicbrokerkeyshipments-post
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      - in: body
        name: Shipment
        description: The shipment
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - The
      - Create
      - Shipmentsales
      - Order
  /api/v1/Orders/{LogicbrokerKey}/Events:
    get:
      summary: Retrieve related events
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetActivityEvent
      x-api-path-slug: apiv1orderslogicbrokerkeyevents-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Related
      - Events
  /api/v1/Orders/{LogicbrokerKey}/Returns:
    get:
      summary: Retrieve a list of returns for an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetReturns
      x-api-path-slug: apiv1orderslogicbrokerkeyreturns-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Returnsan
      - Order
    post:
      summary: The create return for sales order.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_CreateReturnForSalesOrder
      x-api-path-slug: apiv1orderslogicbrokerkeyreturns-post
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      - in: body
        name: Return
        description: The shipment
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - The
      - Create
      - Returnsales
      - Order
  /api/v1/Orders/{LogicbrokerKey}/EDI:
    get:
      summary: Retrieve EDI
      description: Returns the latest EDI related to this document that was either
        sent or received by Logicbroker. The EDI output may also contain other documents
        that were in the same batch.
      operationId: Order_GetDocumentEDI
      x-api-path-slug: apiv1orderslogicbrokerkeyedi-get
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
  /api/v1/Orders/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Order_Import
      x-api-path-slug: apiv1ordersimport-post
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
        description: Return order list instead of saving
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
  /api/v1/Orders/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.logicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Order_GetDocumentExportToken
      x-api-path-slug: apiv1ordersexport-get
      parameters:
      - in: query
        name: Delimiter
        description: The column delimiter to use for CSV export
      - in: query
        name: Fields
        description: The fields to export
      - in: query
        name: FileType
        description: Valid options are csv, xlsx, xml, json and legacy
      - in: query
        name: Filter.advanced
        description: Advanced query options
      - in: query
        name: Filter.from
        description: Beginning of time search window
      - in: query
        name: Filter.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: Filter.page
        description: Page number
      - in: query
        name: Filter.pageSize
        description: Page size
      - in: query
        name: Filter.partnerPO
        description: The partners purchase order number
      - in: query
        name: Filter.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: Filter.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: Filter.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: Filter.status
        description: The status of the document
      - in: query
        name: Filter.to
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
  /api/v1/Orders/{LogicbrokerKey}/PickList:
    get:
      summary: Get pick list for one order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetOrderPickList
      x-api-path-slug: apiv1orderslogicbrokerkeypicklist-get
      parameters:
      - in: query
        name: FileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: path
        name: LogicbrokerKey
        description: The logicbroker Key
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Pick
      - Listone
      - Order
  /api/v1/Orders/PickList:
    get:
      summary: Get pick lists for multiple orders
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetOrderPickListToken
      x-api-path-slug: apiv1orderspicklist-get
      parameters:
      - in: query
        name: FileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker Keys
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Pick
      - Listsmultiple
      - Orders
  /api/v1/Orders/{LogicbrokerKey}:
    get:
      summary: Retrieve an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetSalesOrderDetails
      x-api-path-slug: apiv1orderslogicbrokerkey-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Order
  /api/v1/Orders/{LogicbrokerKey}/Status:
    get:
      summary: Retrieve order status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetSalesOrderStatus
      x-api-path-slug: apiv1orderslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Order
      - Status
  /api/v1/Orders/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Update order status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_UpdateSalesOrderStatus
      x-api-path-slug: apiv1orderslogicbrokerkeystatusstatus-put
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
      - Order
      - Status
  /api/v1/Orders/{LogicbrokerKey}/ShippingOptions:
    get:
      summary: Get shipping/tracking label options.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Order_GetShippingOptions
      x-api-path-slug: apiv1orderslogicbrokerkeyshippingoptions-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Tracking
      - Label
      - Options
  /api/v1/Orders/{LogicbrokerKey}/TrackingLabel:
    post:
      summary: Generate a tracking label for a given package
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Order_CreateTrackingLabel
      x-api-path-slug: apiv1orderslogicbrokerkeytrackinglabel-post
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      - in: body
        name: package
        description: Package details
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: useSenderAccount
        description: Set to true to use the senders shipping account
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Tracking
      - Labela
      - Given
      - Package
  /api/v1/Partners:
    get:
      summary: Retrieve a list of trading partners.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Partner_GetPartners
      x-api-path-slug: apiv1partners-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Trading
      - Partners
  /api/v1/Product/{partnerId}:
    post:
      summary: Import product from CSV.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Product_Upload
      x-api-path-slug: apiv1productpartnerid-post
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
      - Import
      - Product
      - From
      - CSV
  /api/v1/Product/{partnerId}/{feedId}:
    get:
      summary: Get product feed status.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_GetFeedStatus
      x-api-path-slug: apiv1productpartneridfeedid-get
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Product
      - Feed
      - Status
    put:
      summary: Send product feed.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_SendFeed
      x-api-path-slug: apiv1productpartneridfeedid-put
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Send
      - Product
      - Feed
    delete:
      summary: Delete product feed.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_DeleteFeed
      x-api-path-slug: apiv1productpartneridfeedid-delete
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Product
      - Feed
  /api/v1/Product/{partnerId}/{feedId}/Items:
    get:
      summary: Get items in the product feed.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_GetFeedItems
      x-api-path-slug: apiv1productpartneridfeediditems-get
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: query
        name: isCompliant
        description: Compliant filter
      - in: query
        name: page
        description: Page number
      - in: query
        name: pageSize
        description: Page size
      - in: path
        name: partnerId
        description: Partner account number
      responses:
        200:
          description: OK
      tags:
      - Items
      - In
      - Product
      - Feed
  /api/v1/Product/{partnerId}/{feedId}/Items/{productId}:
    get:
      summary: Get product feed item.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_GetFeedItem
      x-api-path-slug: apiv1productpartneridfeediditemsproductid-get
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      - in: path
        name: productId
        description: Product identifier within the feed
      responses:
        200:
          description: OK
      tags:
      - Product
      - Feed
      - Item
    put:
      summary: Update product feed item.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_UpdateFeedItem
      x-api-path-slug: apiv1productpartneridfeediditemsproductid-put
      parameters:
      - in: body
        name: data
        description: Data fields to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      - in: path
        name: productId
        description: Product identifier within the feed
      responses:
        200:
          description: OK
      tags:
      - Product
      - Feed
      - Item
    delete:
      summary: Remove product feed item.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Product_RemoveFeedItem
      x-api-path-slug: apiv1productpartneridfeediditemsproductid-delete
      parameters:
      - in: path
        name: feedId
        description: Feed identifier
      - in: path
        name: partnerId
        description: Partner account number
      - in: path
        name: productId
        description: Product identifier within the feed
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Product
      - Feed
      - Item
  /api/v1/Returns/{LogicbrokerKey}:
    get:
      summary: Get return details
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_GetReturn
      x-api-path-slug: apiv1returnslogicbrokerkey-get
      parameters:
      - in: path
        name: LogicbrokerKey
      responses:
        200:
          description: OK
      tags:
      - Return
      - Details
  /api/v1/Returns/CustomXML:
    post:
      summary: Create return(s) based on custom XML.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_UploadCustomXml
      x-api-path-slug: apiv1returnscustomxml-post
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
      - Return(s)
      - Based
      - "On"
      - Custom
      - XML
  /api/v1/Returns/Request:
    post:
      summary: Request a return
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_CreateReturnRequest
      x-api-path-slug: apiv1returnsrequest-post
      parameters:
      - in: body
        name: Return
        description: Return object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Return
  /api/v1/Returns:
    get:
      summary: Search returns
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_SearchReturns
      x-api-path-slug: apiv1returns-get
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
      - Returns
    post:
      summary: Create a return
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_CreateReturn
      x-api-path-slug: apiv1returns-post
      parameters:
      - in: body
        name: Return
        description: Return object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Return
  /api/v1/Returns/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Update return status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_UpdateReturnStatus
      x-api-path-slug: apiv1returnslogicbrokerkeystatusstatus-put
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
      - Return
      - Status
  /api/v1/Returns/{LogicbrokerKey}/Status:
    get:
      summary: Retrieve return status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Return_GetReturnStatus
      x-api-path-slug: apiv1returnslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Return
      - Status
  /api/v1/Returns/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Return_GetDocumentExportToken
      x-api-path-slug: apiv1returnsexport-get
      parameters:
      - in: query
        name: delimiter
        description: The column delimiter to use for CSV export
      - in: query
        name: fields
        description: The fields to export
      - in: query
        name: fileType
        description: Valid options are csv, xlsx, xml, and json
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
  /api/v1/Returns/{LogicbrokerKey}/EDI:
    get:
      summary: Retrieve EDI
      description: Returns the latest EDI related to this document that was either
        sent or received by Logicbroker. The EDI output may also contain other documents
        that were in the same batch.
      operationId: Return_GetDocumentEDI
      x-api-path-slug: apiv1returnslogicbrokerkeyedi-get
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
  /api/v1/Returns/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Return_Import
      x-api-path-slug: apiv1returnsimport-post
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
  /api/v1/Shipments/CustomXML:
    post:
      summary: Create shipment(s) based on custom XML.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_UploadCustomXml
      x-api-path-slug: apiv1shipmentscustomxml-post
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
      - Shipment(s)
      - Based
      - "On"
      - Custom
      - XML
  /api/v1/Shipments:
    get:
      summary: Get shipments for given filters
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_SearchShipment
      x-api-path-slug: apiv1shipments-get
      parameters:
      - in: query
        name: Filters.advanced
        description: Advanced query options
      - in: query
        name: Filters.from
        description: Beginning of time search window
      - in: query
        name: Filters.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: Filters.page
        description: Page number
      - in: query
        name: Filters.pageSize
        description: Page size
      - in: query
        name: Filters.partnerPO
        description: The partners purchase order number
      - in: query
        name: Filters.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: Filters.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: Filters.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: Filters.status
        description: The status of the document
      - in: query
        name: Filters.to
        description: End of time search window
      responses:
        200:
          description: OK
      tags:
      - Shipmentsgiven
      - Filters
    post:
      summary: Create a new shipment
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_CreateShipment
      x-api-path-slug: apiv1shipments-post
      parameters:
      - in: body
        name: Shipment
        description: The shipment to save
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Shipment
  /api/v1/Shipments/{LogicbrokerKey}/Events:
    get:
      summary: Retrieve related events
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetActivityEvent
      x-api-path-slug: apiv1shipmentslogicbrokerkeyevents-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Related
      - Events
  /api/v1/Shipments/{LogicbrokerKey}/EDI:
    get:
      summary: Retrieve EDI
      description: Returns the latest EDI related to this document that was either
        sent or received by Logicbroker. The EDI output may also contain other documents
        that were in the same batch.
      operationId: Shipment_GetDocumentEDI
      x-api-path-slug: apiv1shipmentslogicbrokerkeyedi-get
      parameters:
      - in: path
        name: LogicbrokerKey
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - EDI
  /api/v1/Shipments/Import:
    post:
      summary: Import from flat file.
      description: Request rate limited to 1 request per second with bursts up to
        10 requests.
      operationId: Shipment_Import
      x-api-path-slug: apiv1shipmentsimport-post
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
  /api/v1/Shipments/Export:
    get:
      summary: Export to CSV/XLSX
      description: "The 'fields' parameter accepts a comma delimited list of JSON
        paths, for example: 'Identifier.logicbrokerKey, BillToAddress.FirstName'.
        It is also possible to rename these fields using syntax like 'DocumentDate
        as Date' or 'DocumentDate Date'.\r\n            You must specify a value for
        either the 'LogicbrokerKeys' parameter or the 'filter' parameter."
      operationId: Shipment_GetDocumentExportToken
      x-api-path-slug: apiv1shipmentsexport-get
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
  /api/v1/Shipments/{LogicbrokerKey}:
    get:
      summary: Get shipment details
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipment
      x-api-path-slug: apiv1shipmentslogicbrokerkey-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Shipment
      - Details
    put:
      summary: Update shipment details
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_UpdateShipment
      x-api-path-slug: apiv1shipmentslogicbrokerkey-put
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      - in: body
        name: Shipment
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipment
      - Details
  /api/v1/Shipments/{LogicbrokerKey}/PackingSlip:
    get:
      summary: Get packing slips for one shipment
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipmentPackingSlip
      x-api-path-slug: apiv1shipmentslogicbrokerkeypackingslip-get
      parameters:
      - in: query
        name: fileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: path
        name: LogicbrokerKey
        description: The logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Packing
      - Slipsone
      - Shipment
  /api/v1/Shipments/PackingSlip:
    get:
      summary: Get packing slips for multiple shipments
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipmentPackingSlipsToken
      x-api-path-slug: apiv1shipmentspackingslip-get
      parameters:
      - in: query
        name: fileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker Keys
      responses:
        200:
          description: OK
      tags:
      - Packing
      - Slipsmultiple
      - Shipments
    post:
      summary: Get packing slips for a shipment before submitting
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipmentPackingSlipsToken
      x-api-path-slug: apiv1shipmentspackingslip-post
      parameters:
      - in: query
        name: fileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: body
        name: shipment
        description: Shipment data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Packing
      - Slipsa
      - Shipment
      - Before
      - Submitting
  /api/v1/Shipments/ShippingLabel:
    get:
      summary: Get shipping labels for multiple shipments
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Shipment_GetShipmentShippingLabelToken
      x-api-path-slug: apiv1shipmentsshippinglabel-get
      parameters:
      - in: query
        name: containerCode
        description: Specific container code
      - in: query
        name: fileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: query
        name: LogicbrokerKeys
        description: The Logicbroker keys
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Labelsmultiple
      - Shipments
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