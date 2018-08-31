---
name: Logicbroker
x-slug: logicbroker
description: Logicbroker provides beautiful technology that unites brands, retailers,
  and the systems they rely on. Harness the latest in cloud and supply chain automation
  technology with unrivaled speed and integration flexibility. We craft the connections
  that enable digital commerce.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
x-kinRank: "7"
x-alexaRank: ""
tags: Logicbroker
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apis.md
specificationVersion: "0.14"
apis:
- name: CommerceAPI - Get acknowledgement details
  x-api-slug: apiv1acknowledgementslogicbrokerkey-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementslogicbrokerkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementslogicbrokerkey-get-openapi.md
- name: CommerceAPI - Create acknowledgement(s) based on custom XML.
  x-api-slug: apiv1acknowledgementscustomxml-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementscustomxml-post-openapi.md
- name: CommerceAPI - Request an acknowledgement from a trading partner
  x-api-slug: apiv1acknowledgementsrequest-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementsrequest-post-openapi.md
- name: CommerceAPI - Search acknowledgements
  x-api-slug: apiv1acknowledgements-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgements-get-openapi.md
- name: CommerceAPI - Create an acknowledgement
  x-api-slug: apiv1acknowledgements-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgements-post-openapi.md
- name: CommerceAPI - Update acknowledgement status
  x-api-slug: apiv1acknowledgementslogicbrokerkeystatusstatus-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementslogicbrokerkeystatusstatus-put-openapi.md
- name: CommerceAPI - Retrieve acknowledgement status
  x-api-slug: apiv1acknowledgementslogicbrokerkeystatus-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementslogicbrokerkeystatus-get-openapi.md
- name: CommerceAPI - Export to CSV/XLSX
  x-api-slug: apiv1acknowledgementsexport-get
  description: "The 'fields' parameter accepts a comma delimited list of JSON paths,
    for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'. It is also
    possible to rename these fields using syntax like 'DocumentDate as Date' or 'DocumentDate
    Date'.\r\n            You must specify a value for either the 'LogicbrokerKeys'
    parameter or the 'filter' parameter."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementsexport-get-openapi.md
- name: CommerceAPI - Retrieve EDI
  x-api-slug: apiv1acknowledgementslogicbrokerkeyedi-get
  description: Returns the latest EDI related to this document that was either sent
    or received by Logicbroker. The EDI output may also contain other documents that
    were in the same batch.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementslogicbrokerkeyedi-get-openapi.md
- name: CommerceAPI - Import from flat file.
  x-api-slug: apiv1acknowledgementsimport-post
  description: Request rate limited to 1 request per second with bursts up to 10 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1acknowledgementsimport-post-openapi.md
- name: CommerceAPI - Get events for given fitlers
  x-api-slug: apiv1activityevents-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1activityevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1activityevents-get-openapi.md
- name: CommerceAPI - Create an activity event.
  x-api-slug: apiv1activityevents-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1activityevents-post-openapi.md
- name: CommerceAPI - Gets the event with the specified id.
  x-api-slug: apiv1activityeventseventid-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1activityeventseventid-get-openapi.md
- name: CommerceAPI - Update activity event
  x-api-slug: apiv1activityeventseventid-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1activityeventseventid-put-openapi.md
- name: CommerceAPI - Gets a list of all possible event types.
  x-api-slug: apiv1activityeventseventtypes-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1activityeventseventtypes-get-openapi.md
- name: CommerceAPI - Get a list of all attachments matching a given filter.
  x-api-slug: apiv1attachments-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1attachments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1attachments-get-openapi.md
- name: CommerceAPI - Upload an attachment
  x-api-slug: apiv1attachments-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1attachments-post-openapi.md
- name: CommerceAPI - Retrieve a file from Logicbroker storage.
  x-api-slug: apiv1attachmentscontainername-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1attachmentscontainername-get-openapi.md
- name: CommerceAPI - Execute custom handler.
  x-api-slug: apiv1documentscriptscriptname-get
  description: Request rate limited to 2 requests per second with bursts up to 25
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1documentscriptscriptname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1documentscriptscriptname-get-openapi.md
- name: CommerceAPI - Execute custom handler.
  x-api-slug: apiv1documentscriptscriptname-post
  description: Request rate limited to 2 requests per second with bursts up to 25
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1documentscriptscriptname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1documentscriptscriptname-post-openapi.md
- name: CommerceAPI - Execute custom handler.
  x-api-slug: apiv1documentscriptscriptname-options
  description: Request rate limited to 2 requests per second with bursts up to 25
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1documentscriptscriptname-options-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1documentscriptscriptname-options-openapi.md
- name: CommerceAPI - Download inventory as CSV.
  x-api-slug: apiv1inventorypartnerid-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventorypartnerid-get-openapi.md
- name: CommerceAPI - Import inventory from CSV.
  x-api-slug: apiv1inventorypartnerid-post
  description: Request rate limited to 1 request per second with bursts up to 2 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventorypartnerid-post-openapi.md
- name: CommerceAPI - Delete all inventory records.
  x-api-slug: apiv1inventorypartnerid-delete
  description: Request rate limited to 1 request every 60 seconds with bursts up to
    2 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventorypartnerid-delete-openapi.md
- name: CommerceAPI - Import inventory from CSV.
  x-api-slug: apiv1inventorybroadcast-post
  description: Request rate limited to 1 request every 60 seconds with bursts up to
    2 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventorybroadcast-post-openapi.md
- name: CommerceAPI - Match items with CSV.
  x-api-slug: apiv1inventorypartneridmatching-post
  description: Request rate limited to 1 request per second with bursts up to 2 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventorypartneridmatching-post-openapi.md
- name: CommerceAPI - Delete all SKU mappings.
  x-api-slug: apiv1inventorypartneridmatching-delete
  description: Request rate limited to 1 request every 60 seconds with bursts up to
    2 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventorypartneridmatching-delete-openapi.md
- name: CommerceAPI - Resend all inventory items.
  x-api-slug: apiv1inventorypartneridresend-put
  description: Request rate limited to 1 request every 5 minutes with bursts up to
    2 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventorypartneridresend-put-openapi.md
- name: CommerceAPI - Get a single item by SKU
  x-api-slug: apiv1inventorypartneriditemsku-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventorypartneriditemsku-get-openapi.md
- name: CommerceAPI - Get the availability of an item across all suppliers.
  x-api-slug: apiv1inventoryavailabilitysku-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1inventoryavailabilitysku-get-openapi.md
- name: CommerceAPI - Create invoice(s) based on custom XML.
  x-api-slug: apiv1invoicescustomxml-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoicescustomxml-post-openapi.md
- name: CommerceAPI - Get invoices based on provided filters
  x-api-slug: apiv1invoices-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoices-get-openapi.md
- name: CommerceAPI - Create a new invoice
  x-api-slug: apiv1invoices-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoices-post-openapi.md
- name: CommerceAPI - Retrieve related events
  x-api-slug: apiv1invoiceslogicbrokerkeyevents-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoiceslogicbrokerkeyevents-get-openapi.md
- name: CommerceAPI - Retrieve EDI
  x-api-slug: apiv1invoiceslogicbrokerkeyedi-get
  description: Returns the latest EDI related to this document that was either sent
    or received by Logicbroker. The EDI output may also contain other documents that
    were in the same batch.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoiceslogicbrokerkeyedi-get-openapi.md
- name: CommerceAPI - Import from flat file.
  x-api-slug: apiv1invoicesimport-post
  description: Request rate limited to 1 request per second with bursts up to 10 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoicesimport-post-openapi.md
- name: CommerceAPI - Export to CSV/XLSX
  x-api-slug: apiv1invoicesexport-get
  description: "The 'fields' parameter accepts a comma delimited list of JSON paths,
    for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'. It is also
    possible to rename these fields using syntax like 'DocumentDate as Date' or 'DocumentDate
    Date'.\r\n            You must specify a value for either the 'LogicbrokerKeys'
    parameter or the 'filter' parameter."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoicesexport-get-openapi.md
- name: CommerceAPI - Returns the invoice with the specified key.
  x-api-slug: apiv1invoiceslogicbrokerkey-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoiceslogicbrokerkey-get-openapi.md
- name: CommerceAPI - Return the current status code of an invoice.
  x-api-slug: apiv1invoiceslogicbrokerkeystatus-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoiceslogicbrokerkeystatus-get-openapi.md
- name: CommerceAPI - Updates an invoice to the specified status.
  x-api-slug: apiv1invoiceslogicbrokerkeystatusstatus-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1invoiceslogicbrokerkeystatusstatus-put-openapi.md
- name: CommerceAPI - Retrieve a list of invoices for an order
  x-api-slug: apiv1orderslogicbrokerkeyinvoices-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyinvoices-get-openapi.md
- name: CommerceAPI - Creates invoice and links with the given order
  x-api-slug: apiv1orderslogicbrokerkeyinvoices-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyinvoices-post-openapi.md
- name: CommerceAPI - Create order(s) based on custom XML.
  x-api-slug: apiv1orderscustomxml-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderscustomxml-post-openapi.md
- name: CommerceAPI - Search orders
  x-api-slug: apiv1orders-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orders-get-openapi.md
- name: CommerceAPI - Create an order
  x-api-slug: apiv1orders-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orders-post-openapi.md
- name: CommerceAPI - Retrieve a list of shipments for an order
  x-api-slug: apiv1orderslogicbrokerkeyshipments-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyshipments-get-openapi.md
- name: CommerceAPI - The create shipment for sales order.
  x-api-slug: apiv1orderslogicbrokerkeyshipments-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyshipments-post-openapi.md
- name: CommerceAPI - Retrieve related events
  x-api-slug: apiv1orderslogicbrokerkeyevents-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyevents-get-openapi.md
- name: CommerceAPI - Retrieve a list of returns for an order
  x-api-slug: apiv1orderslogicbrokerkeyreturns-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyreturns-get-openapi.md
- name: CommerceAPI - The create return for sales order.
  x-api-slug: apiv1orderslogicbrokerkeyreturns-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyreturns-post-openapi.md
- name: CommerceAPI - Retrieve EDI
  x-api-slug: apiv1orderslogicbrokerkeyedi-get
  description: Returns the latest EDI related to this document that was either sent
    or received by Logicbroker. The EDI output may also contain other documents that
    were in the same batch.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyedi-get-openapi.md
- name: CommerceAPI - Import from flat file.
  x-api-slug: apiv1ordersimport-post
  description: Request rate limited to 1 request per second with bursts up to 10 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1ordersimport-post-openapi.md
- name: CommerceAPI - Export to CSV/XLSX
  x-api-slug: apiv1ordersexport-get
  description: "The 'fields' parameter accepts a comma delimited list of JSON paths,
    for example: 'Identifier.logicbrokerKey, BillToAddress.FirstName'. It is also
    possible to rename these fields using syntax like 'DocumentDate as Date' or 'DocumentDate
    Date'.\r\n            You must specify a value for either the 'LogicbrokerKeys'
    parameter or the 'filter' parameter."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1ordersexport-get-openapi.md
- name: CommerceAPI - Get pick list for one order
  x-api-slug: apiv1orderslogicbrokerkeypicklist-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeypicklist-get-openapi.md
- name: CommerceAPI - Get pick lists for multiple orders
  x-api-slug: apiv1orderspicklist-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderspicklist-get-openapi.md
- name: CommerceAPI - Retrieve an order
  x-api-slug: apiv1orderslogicbrokerkey-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkey-get-openapi.md
- name: CommerceAPI - Retrieve order status
  x-api-slug: apiv1orderslogicbrokerkeystatus-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeystatus-get-openapi.md
- name: CommerceAPI - Update order status
  x-api-slug: apiv1orderslogicbrokerkeystatusstatus-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeystatusstatus-put-openapi.md
- name: CommerceAPI - Get shipping/tracking label options.
  x-api-slug: apiv1orderslogicbrokerkeyshippingoptions-get
  description: Request rate limited to 2 requests per second with bursts up to 25
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeyshippingoptions-get-openapi.md
- name: CommerceAPI - Generate a tracking label for a given package
  x-api-slug: apiv1orderslogicbrokerkeytrackinglabel-post
  description: Request rate limited to 2 requests per second with bursts up to 25
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1orderslogicbrokerkeytrackinglabel-post-openapi.md
- name: CommerceAPI - Retrieve a list of trading partners.
  x-api-slug: apiv1partners-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1partners-get-openapi.md
- name: CommerceAPI - Import product from CSV.
  x-api-slug: apiv1productpartnerid-post
  description: Request rate limited to 1 request per second with bursts up to 10 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1productpartnerid-post-openapi.md
- name: CommerceAPI - Get product feed status.
  x-api-slug: apiv1productpartneridfeedid-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1productpartneridfeedid-get-openapi.md
- name: CommerceAPI - Send product feed.
  x-api-slug: apiv1productpartneridfeedid-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1productpartneridfeedid-put-openapi.md
- name: CommerceAPI - Delete product feed.
  x-api-slug: apiv1productpartneridfeedid-delete
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1productpartneridfeedid-delete-openapi.md
- name: CommerceAPI - Get items in the product feed.
  x-api-slug: apiv1productpartneridfeediditems-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1productpartneridfeediditems-get-openapi.md
- name: CommerceAPI - Get product feed item.
  x-api-slug: apiv1productpartneridfeediditemsproductid-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1productpartneridfeediditemsproductid-get-openapi.md
- name: CommerceAPI - Update product feed item.
  x-api-slug: apiv1productpartneridfeediditemsproductid-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1productpartneridfeediditemsproductid-put-openapi.md
- name: CommerceAPI - Remove product feed item.
  x-api-slug: apiv1productpartneridfeediditemsproductid-delete
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1productpartneridfeediditemsproductid-delete-openapi.md
- name: CommerceAPI - Get return details
  x-api-slug: apiv1returnslogicbrokerkey-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returnslogicbrokerkey-get-openapi.md
- name: CommerceAPI - Create return(s) based on custom XML.
  x-api-slug: apiv1returnscustomxml-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returnscustomxml-post-openapi.md
- name: CommerceAPI - Request a return
  x-api-slug: apiv1returnsrequest-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returnsrequest-post-openapi.md
- name: CommerceAPI - Search returns
  x-api-slug: apiv1returns-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returns-get-openapi.md
- name: CommerceAPI - Create a return
  x-api-slug: apiv1returns-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returns-post-openapi.md
- name: CommerceAPI - Update return status
  x-api-slug: apiv1returnslogicbrokerkeystatusstatus-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returnslogicbrokerkeystatusstatus-put-openapi.md
- name: CommerceAPI - Retrieve return status
  x-api-slug: apiv1returnslogicbrokerkeystatus-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returnslogicbrokerkeystatus-get-openapi.md
- name: CommerceAPI - Export to CSV/XLSX
  x-api-slug: apiv1returnsexport-get
  description: "The 'fields' parameter accepts a comma delimited list of JSON paths,
    for example: 'Identifier.LogicbrokerKey, BillToAddress.FirstName'. It is also
    possible to rename these fields using syntax like 'DocumentDate as Date' or 'DocumentDate
    Date'.\r\n            You must specify a value for either the 'LogicbrokerKeys'
    parameter or the 'filter' parameter."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returnsexport-get-openapi.md
- name: CommerceAPI - Retrieve EDI
  x-api-slug: apiv1returnslogicbrokerkeyedi-get
  description: Returns the latest EDI related to this document that was either sent
    or received by Logicbroker. The EDI output may also contain other documents that
    were in the same batch.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returnslogicbrokerkeyedi-get-openapi.md
- name: CommerceAPI - Import from flat file.
  x-api-slug: apiv1returnsimport-post
  description: Request rate limited to 1 request per second with bursts up to 10 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1returnsimport-post-openapi.md
- name: CommerceAPI - Create shipment(s) based on custom XML.
  x-api-slug: apiv1shipmentscustomxml-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentscustomxml-post-openapi.md
- name: CommerceAPI - Get shipments for given filters
  x-api-slug: apiv1shipments-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipments-get-openapi.md
- name: CommerceAPI - Create a new shipment
  x-api-slug: apiv1shipments-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipments-post-openapi.md
- name: CommerceAPI - Retrieve related events
  x-api-slug: apiv1shipmentslogicbrokerkeyevents-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentslogicbrokerkeyevents-get-openapi.md
- name: CommerceAPI - Retrieve EDI
  x-api-slug: apiv1shipmentslogicbrokerkeyedi-get
  description: Returns the latest EDI related to this document that was either sent
    or received by Logicbroker. The EDI output may also contain other documents that
    were in the same batch.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentslogicbrokerkeyedi-get-openapi.md
- name: CommerceAPI - Import from flat file.
  x-api-slug: apiv1shipmentsimport-post
  description: Request rate limited to 1 request per second with bursts up to 10 requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentsimport-post-openapi.md
- name: CommerceAPI - Export to CSV/XLSX
  x-api-slug: apiv1shipmentsexport-get
  description: "The 'fields' parameter accepts a comma delimited list of JSON paths,
    for example: 'Identifier.logicbrokerKey, BillToAddress.FirstName'. It is also
    possible to rename these fields using syntax like 'DocumentDate as Date' or 'DocumentDate
    Date'.\r\n            You must specify a value for either the 'LogicbrokerKeys'
    parameter or the 'filter' parameter."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentsexport-get-openapi.md
- name: CommerceAPI - Get shipment details
  x-api-slug: apiv1shipmentslogicbrokerkey-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentslogicbrokerkey-get-openapi.md
- name: CommerceAPI - Update shipment details
  x-api-slug: apiv1shipmentslogicbrokerkey-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentslogicbrokerkey-put-openapi.md
- name: CommerceAPI - Get packing slips for one shipment
  x-api-slug: apiv1shipmentslogicbrokerkeypackingslip-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentslogicbrokerkeypackingslip-get-openapi.md
- name: CommerceAPI - Get packing slips for multiple shipments
  x-api-slug: apiv1shipmentspackingslip-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentspackingslip-get-openapi.md
- name: CommerceAPI - Get packing slips for a shipment before submitting
  x-api-slug: apiv1shipmentspackingslip-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentspackingslip-post-openapi.md
- name: CommerceAPI - Get shipping labels for multiple shipments
  x-api-slug: apiv1shipmentsshippinglabel-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentsshippinglabel-get-openapi.md
- name: CommerceAPI - Get shipping labels for a shipment before submitting
  x-api-slug: apiv1shipmentsshippinglabel-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentsshippinglabel-post-openapi.md
- name: CommerceAPI - Get shipping labels for one shipment.
  x-api-slug: apiv1shipmentslogicbrokerkeyshippinglabel-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentslogicbrokerkeyshippinglabel-get-openapi.md
- name: CommerceAPI - Get shipment status
  x-api-slug: apiv1shipmentslogicbrokerkeystatus-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentslogicbrokerkeystatus-get-openapi.md
- name: CommerceAPI - Update shipment status
  x-api-slug: apiv1shipmentslogicbrokerkeystatusstatus-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentslogicbrokerkeystatusstatus-put-openapi.md
- name: CommerceAPI - Gets a new SSCC18 container code.
  x-api-slug: apiv1shipmentscontainercode-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1shipmentscontainercode-get-openapi.md
- name: CommerceAPI - Get configured document statuses for each document
  x-api-slug: apiv1statuses-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1statuses-get-openapi.md
- name: CommerceAPI - Get configured document statuses for each document
  x-api-slug: apiv1statusesdocumenttype-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1statusesdocumenttype-get-openapi.md
- name: CommerceAPI - Get list of webhooks
  x-api-slug: apiv1webhooks-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1webhooks-get-openapi.md
- name: CommerceAPI - Create a new webhook
  x-api-slug: apiv1webhooks-post
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1webhooks-post-openapi.md
- name: CommerceAPI - Get webhook details
  x-api-slug: apiv1webhookswebhookid-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1webhookswebhookid-get-openapi.md
- name: CommerceAPI - Update a webhook
  x-api-slug: apiv1webhookswebhookid-put
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1webhookswebhookid-put-openapi.md
- name: CommerceAPI - Delete a webhook.
  x-api-slug: apiv1webhookswebhookid-delete
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1webhookswebhookid-delete-openapi.md
- name: CommerceAPI - Test a webhook endpoint.
  x-api-slug: apiv1webhookswebhookidtest-get
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/logicbroker-logo.png
  humanURL: https://www.logicbroker.com/
  baseURL: https://stage.commerceapi.io//
  tags: Commerce, Retail
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/logicbroker/master/_listings/logicbroker/apiv1webhookswebhookidtest-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.logicbroker.com/feed/
- type: x-developer
  url: https://dev.logicbroker.com/
- type: x-openapi
  url: https://stage.commerceapi.io/swagger/docs/v1
- type: x-api-gallery
  url: http://kentico.cloud.api.gallery.streamdata.io
- type: x-documentation
  url: https://stage.commerceapi.io/swagger/ui/index
- type: x-website
  url: https://www.logicbroker.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---