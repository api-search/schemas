---
description: Describes an Amazon Aurora DB cluster
layout: schema
name: DBCluster
properties_list:
- description: The user-supplied identifier for the DB cluster
  name: dBClusterIdentifier
  type: string
- description: The Amazon Resource Name (ARN) for the DB cluster
  name: dBClusterArn
  type: string
- description: The current state of the DB cluster
  name: status
  type: string
- description: The database engine for the DB cluster
  name: engine
  type: string
- description: The version of the database engine
  name: engineVersion
  type: string
- description: The name of the initial database
  name: databaseName
  type: string
- description: The master username for the DB cluster
  name: masterUsername
  type: string
- description: The DNS address of the primary instance of the DB cluster
  name: endpoint
  type: string
- description: The reader endpoint for the DB cluster
  name: readerEndpoint
  type: string
- description: The port that the database engine is listening on
  name: port
  type: integer
- description: The list of DB instances that are part of the cluster
  name: dBClusterMembers
  type: array
- description: The Availability Zones the DB cluster is associated with
  name: availabilityZones
  type: array
- description: The number of days for which automatic DB snapshots are retained
  name: backupRetentionPeriod
  type: integer
- description: Whether the DB cluster is encrypted
  name: storageEncrypted
  type: boolean
- description: Whether the DB cluster has instances in multiple AZs
  name: multiAZ
  type: boolean
- description: The time when the DB cluster was created
  name: clusterCreateTime
  type: string
- description: The current allocated storage size in GiB for the cluster
  name: allocatedStorage
  type: integer
- description: Tags assigned to the DB cluster
  name: tags
  type: array
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-db-cluster-schema.json
slug: amazon-rds-openapi-db-cluster
source_filename: amazon-rds-openapi-db-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-db-cluster-schema.json\",\n  \"title\": \"DBCluster\",\n  \"description\": \"Describes an Amazon Aurora DB cluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied identifier for the DB cluster\"\n    },\n    \"dBClusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB cluster\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the DB cluster\"\n    },\n    \"engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine for the DB cluster\"\n    },\n    \"engineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the database\
  \ engine\"\n    },\n    \"databaseName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the initial database\"\n    },\n    \"masterUsername\": {\n      \"type\": \"string\",\n      \"description\": \"The master username for the DB cluster\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS address of the primary instance of the DB cluster\"\n    },\n    \"readerEndpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The reader endpoint for the DB cluster\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port that the database engine is listening on\"\n    },\n    \"dBClusterMembers\": {\n      \"type\": \"array\",\n      \"description\": \"The list of DB instances that are part of the cluster\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"dBInstanceIdentifier\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The instance identifier for the cluster member\"\n          },\n          \"isClusterWriter\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the cluster member is the primary instance\"\n          },\n          \"dBClusterParameterGroupStatus\": {\n            \"type\": \"string\",\n            \"description\": \"The status of the parameter group for this member\"\n          }\n        }\n      }\n    },\n    \"availabilityZones\": {\n      \"type\": \"array\",\n      \"description\": \"The Availability Zones the DB cluster is associated with\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"backupRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days for which automatic DB snapshots are retained\"\n    },\n    \"storageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB cluster is encrypted\"\n    },\n    \"multiAZ\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether the DB cluster has instances in multiple AZs\"\n    },\n    \"clusterCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the DB cluster was created\"\n    },\n    \"allocatedStorage\": {\n      \"type\": \"integer\",\n      \"description\": \"The current allocated storage size in GiB for the cluster\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the DB cluster\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-db-cluster-schema.json
tags:
- AWS
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: DBCluster
---
