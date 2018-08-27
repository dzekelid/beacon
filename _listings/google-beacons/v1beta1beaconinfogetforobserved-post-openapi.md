---
swagger: "2.0"
x-collection-name: Google Beacons
x-complete: 0
info:
  title: Google Proximity Beacon API Get Observed Beacon Info
  description: |-
    Given one or more beacon observations, returns any beacon information
    and attachments accessible to your application. Authorize by using the
    [API key](https://developers.google.com/beacons/proximity/how-tos/authorizing#APIKey)
    for the application.
  contact:
    name: Google
    url: https://google.com
  version: v1beta1
host: proximitybeacon.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1beta1/beaconinfo:getforobserved:
    post:
      summary: Get Observed Beacon Info
      description: |-
        Given one or more beacon observations, returns any beacon information
        and attachments accessible to your application. Authorize by using the
        [API key](https://developers.google.com/beacons/proximity/how-tos/authorizing#APIKey)
        for the application.
      operationId: proximitybeacon.beaconinfo.getforobserved
      x-api-path-slug: v1beta1beaconinfogetforobserved-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Beacon
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