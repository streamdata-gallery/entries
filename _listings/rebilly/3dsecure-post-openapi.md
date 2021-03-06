---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Create a ThreeDSecure entry
  description: Create a ThreeDSecure entry
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dsecure:
    get:
      summary: Retrieve a list of ThreeDSecure entries
      description: Retrieve a list of ThreeDSecure entries
      operationId: 3dsecure.get
      x-api-path-slug: 3dsecure-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - ThreeDSecure
      - Entries
    post:
      summary: Create a ThreeDSecure entry
      description: Create a ThreeDSecure entry
      operationId: 3dsecure.post
      x-api-path-slug: 3dsecure-post
      parameters:
      - in: body
        name: body
        description: ThreeDSecure resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ThreeDSecure
      - Entry
  /3dsecure/{id}:
    get:
      summary: Retrieve a ThreeDSecure entry
      description: Retrieve a ThreeDSecure entry with specified identifier string
      operationId: 3dsecure.id.get
      x-api-path-slug: 3dsecureid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - ThreeDSecure
      - Entry
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