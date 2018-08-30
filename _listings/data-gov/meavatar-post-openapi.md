---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Me Avatar
  description: Upload a new avatar
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
    get:
      summary: Get Datasets Community Resources Community
      description: Retrieve a community resource given its identifier
      operationId: getDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-get
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
    put:
      summary: Put Datasets Community Resources Community
      description: Update a given community resource
      operationId: putDatasetsCommunityResourcesCommunity
      x-api-path-slug: datasetscommunity-resourcescommunity-put
      parameters:
      - in: path
        name: community
        description: The community resource unique identifier
      - in: query
        name: dataset
        description: The dataset ID or slug
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
      - Community
  /datasets/community_resources/{community}/upload/:
    post:
      summary: Add Datasets Community Resources Community Upload
      description: Update the file related to a given community resource
      operationId: postDatasetsCommunityResourcesCommunityUpload
      x-api-path-slug: datasetscommunity-resourcescommunityupload-post
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
      - Upload
  /datasets/frequencies/:
    get:
      summary: Get Datasets Frequencies
      description: List all available frequencies
      operationId: getDatasetsFrequencies
      x-api-path-slug: datasetsfrequencies-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Frequencies
  /datasets/full/:
    get:
      summary: Get Datasets Full
      description: ""
      operationId: getDatasetsFull
      x-api-path-slug: datasetsfull-get
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
      - Full
  /datasets/licenses/:
    get:
      summary: Get Datasets Licenses
      description: List all available licenses
      operationId: getDatasetsLicenses
      x-api-path-slug: datasetslicenses-get
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Licenses
  /datasets/suggest/:
    get:
      summary: Get Datasets Suggest
      description: Suggest datasets
      operationId: getDatasetsSuggest
      x-api-path-slug: datasetssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Suggest
  /datasets/suggest/formats/:
    get:
      summary: Get Datasets Suggest Formats
      description: Suggest file formats
      operationId: getDatasetsSuggestFormats
      x-api-path-slug: datasetssuggestformats-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Suggest
      - Formats
  /datasets/{dataset}/:
    delete:
      summary: Delete Datasets Dataset
      description: Delete a dataset given its identifier
      operationId: deleteDatasetsDataset
      x-api-path-slug: datasetsdataset-delete
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
    get:
      summary: Get Datasets Dataset
      description: Get a dataset given its identifier
      operationId: getDatasetsDataset
      x-api-path-slug: datasetsdataset-get
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
    put:
      summary: Put Datasets Dataset
      description: Update a dataset given its identifier
      operationId: putDatasetsDataset
      x-api-path-slug: datasetsdataset-put
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
  /datasets/{dataset}/badges/:
    post:
      summary: Add Datasets Dataset Badges
      description: Create a new badge for a given dataset
      operationId: postDatasetsDatasetBadges
      x-api-path-slug: datasetsdatasetbadges-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Badges
  /datasets/{dataset}/badges/{badge_kind}/:
    delete:
      summary: Delete Datasets Dataset Badges Badge Kind
      description: Delete a badge for a given dataset
      operationId: deleteDatasetsDatasetBadgesBadgeKind
      x-api-path-slug: datasetsdatasetbadgesbadge-kind-delete
      parameters:
      - in: path
        name: badge_kind
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Badges
      - Badge
      - Kind
  /datasets/{dataset}/featured/:
    delete:
      summary: Delete Datasets Dataset Featured
      description: Unmark the dataset as featured
      operationId: deleteDatasetsDatasetFeatured
      x-api-path-slug: datasetsdatasetfeatured-delete
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Featured
    post:
      summary: Add Datasets Dataset Featured
      description: Mark the dataset as featured
      operationId: postDatasetsDatasetFeatured
      x-api-path-slug: datasetsdatasetfeatured-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Featured
  /datasets/{dataset}/full/:
    get:
      summary: Get Datasets Dataset Full
      description: Get a dataset given its identifier
      operationId: getDatasetsDatasetFull
      x-api-path-slug: datasetsdatasetfull-get
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Full
  /datasets/{dataset}/resources/:
    post:
      summary: Add Datasets Dataset Resources
      description: Create a new resource for a given dataset
      operationId: postDatasetsDatasetResources
      x-api-path-slug: datasetsdatasetresources-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
    put:
      summary: Put Datasets Dataset Resources
      description: Reorder resources
      operationId: putDatasetsDatasetResources
      x-api-path-slug: datasetsdatasetresources-put
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
  /datasets/{dataset}/resources/{rid}/:
    delete:
      summary: Delete Datasets Dataset Resources R
      description: Delete a given resource on a given dataset
      operationId: deleteDatasetsDatasetResourcesR
      x-api-path-slug: datasetsdatasetresourcesrid-delete
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: path
        name: rid
        description: The resource unique identifier
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
      - R
    put:
      summary: Put Datasets Dataset Resources R
      description: Update a given resource on a given dataset
      operationId: putDatasetsDatasetResourcesR
      x-api-path-slug: datasetsdatasetresourcesrid-put
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: rid
        description: The resource unique identifier
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
      - R
  /datasets/{dataset}/resources/{rid}/upload/:
    post:
      summary: Add Datasets Dataset Resources R Upload
      description: Upload a file related to a given resource on a given dataset
      operationId: postDatasetsDatasetResourcesRUpload
      x-api-path-slug: datasetsdatasetresourcesridupload-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: path
        name: rid
        description: The resource unique identifier
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Resources
      - R
      - Upload
  /datasets/{dataset}/upload/:
    post:
      summary: Add Datasets Dataset Upload
      description: Upload a new dataset resource
      operationId: postDatasetsDatasetUpload
      x-api-path-slug: datasetsdatasetupload-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Upload
  /datasets/{dataset}/upload/community/:
    post:
      summary: Add Datasets Dataset Upload Community
      description: Upload a new community resource
      operationId: postDatasetsDatasetUploadCommunity
      x-api-path-slug: datasetsdatasetuploadcommunity-post
      parameters:
      - in: path
        name: dataset
        description: The dataset ID or slug
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - Dataset
      - Upload
      - Community
  /datasets/{id}/followers/:
    delete:
      summary: Delete Datasets  Followers
      description: Unfollow an object given its ID
      operationId: deleteDatasetsFollowers
      x-api-path-slug: datasetsidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - ""
      - Followers
    get:
      summary: Get Datasets  Followers
      description: List all followers for a given object
      operationId: getDatasetsFollowers
      x-api-path-slug: datasetsidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - ""
      - Followers
    post:
      summary: Add Datasets  Followers
      description: Follow an object given its ID
      operationId: postDatasetsFollowers
      x-api-path-slug: datasetsidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Datasets
      - ""
      - Followers
  /discussions/:
    get:
      summary: Get Discussions
      description: List all Discussions
      operationId: getDiscussions
      x-api-path-slug: discussions-get
      parameters:
      - in: query
        name: closed
        description: Filters discussions on their closed status if specified
      - in: query
        name: for
        description: Filter discussions for a given subject
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
      - Discussions
    post:
      summary: Add Discussions
      description: Create a new Discussion
      operationId: postDiscussions
      x-api-path-slug: discussions-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Discussions
  /discussions/{id}/:
    delete:
      summary: Delete Discussions
      description: Delete a discussion given its ID
      operationId: deleteDiscussions
      x-api-path-slug: discussionsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Discussions
    get:
      summary: Get Discussions
      description: Get a discussion given its ID
      operationId: getDiscussions
      x-api-path-slug: discussionsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Discussions
    post:
      summary: Add Discussions
      description: Add comment and optionnaly close a discussion given its ID
      operationId: postDiscussions
      x-api-path-slug: discussionsid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Discussions
  /harvest/backends:
    get:
      summary: Get Harvest Backends
      description: List all available harvest backends
      operationId: getHarvestBackends
      x-api-path-slug: harvestbackends-get
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Backends
  /harvest/job/{ident}/:
    get:
      summary: Get Harvest Job
      description: List all jobs for a given source
      operationId: getHarvestJobEnt
      x-api-path-slug: harvestjobident-get
      parameters:
      - in: path
        name: ident
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Job
      - Ent
  /harvest/job_status:
    get:
      summary: Get Harvest Job Status
      description: List all available harvesters
      operationId: getHarvestJobStatus
      x-api-path-slug: harvestjob-status-get
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Job
      - Status
  /harvest/source/{ident}:
    delete:
      summary: Delete Harvest Source Ent
      description: ""
      operationId: deleteHarvestSourceEnt
      x-api-path-slug: harvestsourceident-delete
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
    get:
      summary: Get Harvest Source Ent
      description: Get a single source given an ID or a slug
      operationId: getHarvestSourceEnt
      x-api-path-slug: harvestsourceident-get
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
  /harvest/source/{ident}/jobs/:
    get:
      summary: Get Harvest Source Ent Jobs
      description: List all jobs for a given source
      operationId: getHarvestSourceEntJobs
      x-api-path-slug: harvestsourceidentjobs-get
      parameters:
      - in: path
        name: ident
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Jobs
  /harvest/source/{ident}/preview:
    get:
      summary: Get Harvest Source Ent Preview
      description: Preview a single harvest source given an ID or a slug
      operationId: getHarvestSourceEntPreview
      x-api-path-slug: harvestsourceidentpreview-get
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Preview
  /harvest/source/{ident}/validate:
    post:
      summary: Add Harvest Source Ent Valate
      description: Validate or reject an harvest source
      operationId: postHarvestSourceEntValate
      x-api-path-slug: harvestsourceidentvalidate-post
      parameters:
      - in: path
        name: ident
        description: A source ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Source
      - Ent
      - Valate
  /harvest/sources/:
    get:
      summary: Get Harvest Sources
      description: List all harvest sources
      operationId: getHarvestSources
      x-api-path-slug: harvestsources-get
      parameters:
      - in: query
        name: owner
        description: The organization or user ID to filter on
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Sources
    post:
      summary: Add Harvest Sources
      description: Create a new harvests source
      operationId: postHarvestSources
      x-api-path-slug: harvestsources-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Harvest
      - Sources
  /issues/:
    get:
      summary: Get Issues
      description: List all Issues
      operationId: getIssues
      x-api-path-slug: issues-get
      parameters:
      - in: query
        name: closed
        description: Filter closed issues
      - in: query
        name: for
        description: Filter issues for a given subject
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
      - Issues
    post:
      summary: Add Issues
      description: Create a new Issue
      operationId: postIssues
      x-api-path-slug: issues-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issues
  /issues/{id}/:
    get:
      summary: Get Issues
      description: Get an issue given its ID
      operationId: getIssues
      x-api-path-slug: issuesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Issues
    post:
      summary: Add Issues
      description: Add comment and optionnaly close an issue given its ID
      operationId: postIssues
      x-api-path-slug: issuesid-post
      parameters:
      - in: path
        name: id
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Issues
  /me/:
    get:
      summary: Get Me
      description: Fetch the current user (me) identity
      operationId: getMe
      x-api-path-slug: me-get
      responses:
        200:
          description: OK
      tags:
      - Me
    put:
      summary: Put Me
      description: Update my profile
      operationId: putMe
      x-api-path-slug: me-put
      responses:
        200:
          description: OK
      tags:
      - Me
  /me/apikey:
    delete:
      summary: Delete Me Apikey
      description: Clear/destroy an apikey
      operationId: deleteMeApikey
      x-api-path-slug: meapikey-delete
      responses:
        200:
          description: OK
      tags:
      - Me
      - Apikey
    post:
      summary: Add Me Apikey
      description: (Re)Generate my API Key
      operationId: postMeApikey
      x-api-path-slug: meapikey-post
      responses:
        200:
          description: OK
      tags:
      - Me
      - Apikey
  /me/avatar:
    post:
      summary: Add Me Avatar
      description: Upload a new avatar
      operationId: postMeAvatar
      x-api-path-slug: meavatar-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Me
      - Avatar
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