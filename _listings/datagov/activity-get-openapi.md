---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Get Activity
  description: Fetch site activity, optionally filterd by user of org
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activity:
    get:
      summary: Get Activity
      description: Fetch site activity, optionally filterd by user of org
      operationId: getActivity
      x-api-path-slug: activity-get
      parameters:
      - in: query
        name: organization
        description: Filter activities for that particular organization
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      - in: query
        name: user
        description: Filter activities for that particular user
      responses:
        200:
          description: OK
      tags:
      - Activity
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