---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Delete Datasets Community Resources Community
  description: Delete a given community resource
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
  /datasets/:
    get:
      summary: Get Datasets
      description: List or search all datasets
      operationId: getDatasets
      x-api-path-slug: datasets-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: extra
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: featured
      - in: query
        name: format
      - in: query
        name: geozone
      - in: query
        name: granularity
      - in: query
        name: license
      - in: query
        name: organization
      - in: query
        name: owner
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      - in: query
        name: tag
      - in: query
        name: temporal_coverage
      responses:
        200:
          description: OK
      tags:
      - Datasets
    post:
      summary: Add Datasets
      description: Create a new dataset
      operationId: postDatasets
      x-api-path-slug: datasets-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
  /datasets/badges/:
    get:
      summary: Get Datasets Badges
      description: List all available dataset badges and their labels
      operationId: getDatasetsBadges
      x-api-path-slug: datasetsbadges-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Badges
  /datasets/checkurl/:
    get:
      summary: Get Datasets Checkurl
      description: Checks that a URL exists and returns metadata
      operationId: getDatasetsCheckurl
      x-api-path-slug: datasetscheckurl-get
      parameters:
      - in: query
        name: group
        description: The dataset related to the URL
      - in: query
        name: url
        description: The URL to check
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Checkurl
  /datasets/community_resources/:
    get:
      summary: Get Datasets Community Resources
      description: List all community resources
      operationId: getDatasetsCommunityResources
      x-api-path-slug: datasetscommunity-resources-get
      parameters:
      - in: query
        name: dataset
        description: Filter activities for that particular dataset
      - in: query
        name: organization
        description: Filter activities for that particular organization
      - in: query
        name: owner
        description: Filter activities for that particular user
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      - in: query
        name: sort
        description: The sorting attribute
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
    post:
      summary: Add Datasets Community Resources
      description: Create a new community resource
      operationId: postDatasetsCommunityResources
      x-api-path-slug: datasetscommunity-resources-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
  /datasets/community_resources/{community}/:
    delete:
      summary: Delete Datasets Community Resources Community
      description: Delete a given community resource
      operationId: deleteDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-delete
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Community
      - Resources
      - Community
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