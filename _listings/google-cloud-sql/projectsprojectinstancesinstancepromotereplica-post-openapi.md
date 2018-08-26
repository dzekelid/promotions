---
swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 0
info:
  title: Google Cloud SQL API Add Projects Project Instances Instance Promotereplica
  description: Promotes the read replica instance to be a stand-alone Cloud SQL instance.
  contact:
    name: Google
    url: https://google.com
  version: v1beta4
host: www.googleapis.com
basePath: /sql/v1beta4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{project}/instances/{instance}/promoteReplica:
    post:
      summary: Add Projects Project Instances Instance Promotereplica
      description: Promotes the read replica instance to be a stand-alone Cloud SQL
        instance.
      operationId: sql.instances.promoteReplica
      x-api-path-slug: projectsprojectinstancesinstancepromotereplica-post
      parameters:
      - in: path
        name: instance
        description: Cloud SQL read replica instance name
      - in: path
        name: project
        description: ID of the project that contains the read replica
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Promotereplica
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