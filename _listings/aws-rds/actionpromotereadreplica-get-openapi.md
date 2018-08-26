---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Promote Read Replica
  version: 1.0.0
  description: Promotes a Read Replica DB instance to a standalone DB instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PromoteReadReplica:
    get:
      summary: Promote Read Replica
      description: Promotes a Read Replica DB instance to a standalone DB instance.
      operationId: promotereadreplica
      x-api-path-slug: actionpromotereadreplica-get
      parameters:
      - in: query
        name: BackupRetentionPeriod
        description: The number of days to retain automated backups
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled,        using the BackupRetentionPeriod parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replicas
  /?Action=PromoteReadReplicaDBCluster:
    get:
      summary: Promote Read Replica D B Cluster
      description: Promotes a Read Replica DB cluster to a standalone DB cluster.
      operationId: promotereadreplicadbcluster
      x-api-path-slug: actionpromotereadreplicadbcluster-get
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The identifier of the DB cluster Read Replica to promote
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replicas
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