---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean List all Volume snapshots
  description: To retrieve only snapshots based on volumes, include the resource_type
    query paramter set to volume, /v2/snapshots?resource_type=volume.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /snapshots:
    get:
      summary: List all Volume snapshots
      description: To retrieve only snapshots based on volumes, include the resource_type
        query paramter set to volume, /v2/snapshots?resource_type=volume.
      operationId: SnapshotsGet3
      x-api-path-slug: snapshots-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: resource_type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Volume
      - Snapshots
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