---
swagger: "2.0"
info:
  title: SalesForce Get Version Search
  description: Executes the specified SOSL search. The search string must be URL-encoded.
  version: 1.0.0
host: na14.salesforce.com
basePath: /services/data
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{version}/search:
    get:
      summary: Get Version Search
      description: Executes the specified SOSL search
      operationId: version.search.get
      responses:
        200:
          description: OK
      tags:
      - version
      - search
definitions: []
x-collection-name: Salesforce
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