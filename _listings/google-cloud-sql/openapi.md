swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 1
info:
  title: Cloud SQL Administration
  description: creates-and-configures-cloud-sql-instances-which-provide-fullymanaged-mysql-databases-
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