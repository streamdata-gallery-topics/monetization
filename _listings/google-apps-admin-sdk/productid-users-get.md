---
swagger: "2.0"
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{productId}/users:
    get:
      summary: Get License Assignment For User
      description: List license assignments for given product of the customer
      operationId: licensing.licenseAssignments.listForProduct
      parameters:
      - in: query
        name: customerId
        description: CustomerId represents the customer for whom licenseassignments
          are queried
      - in: query
        name: maxResults
        description: Maximum number of campaigns to return at one time
      - in: query
        name: pageToken
        description: Token to fetch the next page
      - in: path
        name: productId
        description: Name for product
      responses:
        200:
          description: OK
      tags:
      - license
definitions: []
x-collection-name: Google Apps Admin SDK
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