---
description: DBCluster schema from Amazon DocumentDB API
layout: schema
name: DBCluster
properties_list:
- description: The identifier of the DB cluster.
  name: DBClusterIdentifier
  type: string
- description: The Amazon Resource Name (ARN) for the DB cluster.
  name: DBClusterArn
  type: string
- description: Specifies the current state of this DB cluster.
  name: Status
  type: string
- description: The database engine used for this DB cluster.
  name: Engine
  type: string
- description: The version of the database engine.
  name: EngineVersion
  type: string
- description: The connection endpoint for the primary instance of the DB cluster.
  name: Endpoint
  type: string
- description: The reader endpoint for the DB cluster.
  name: ReaderEndpoint
  type: string
- description: The port that the database engine is listening on.
  name: Port
  type: integer
- description: The master username for the DB cluster.
  name: MasterUsername
  type: string
- description: The DB subnet group associated with the DB cluster.
  name: DBSubnetGroup
  type: string
- description: Specifies whether the DB cluster is encrypted.
  name: StorageEncrypted
  type: boolean
- description: The number of days for which automatic DB snapshots are retained.
  name: BackupRetentionPeriod
  type: integer
- description: The time when the DB cluster was created.
  name: ClusterCreateTime
  type: string
- description: The list of instances that make up the DB cluster.
  name: DBClusterMembers
  type: array
provider_name: Amazon DocumentDB
provider_slug: amazon-documentdb
schema_file: json-schema/documentdb-openapi-db-cluster-schema.json
slug: documentdb-openapi-db-cluster
source_filename: documentdb-openapi-db-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/json-schema/documentdb-openapi-db-cluster-schema.json\",\n  \"title\": \"DBCluster\",\n  \"description\": \"DBCluster schema from Amazon DocumentDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the DB cluster.\"\n    },\n    \"DBClusterArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB cluster.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the current state of this DB cluster.\"\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine used for this DB cluster.\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version\
  \ of the database engine.\"\n    },\n    \"Endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The connection endpoint for the primary instance of the DB cluster.\"\n    },\n    \"ReaderEndpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The reader endpoint for the DB cluster.\"\n    },\n    \"Port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port that the database engine is listening on.\"\n    },\n    \"MasterUsername\": {\n      \"type\": \"string\",\n      \"description\": \"The master username for the DB cluster.\"\n    },\n    \"DBSubnetGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The DB subnet group associated with the DB cluster.\"\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the DB cluster is encrypted.\"\n    },\n    \"BackupRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days for which automatic\
  \ DB snapshots are retained.\"\n    },\n    \"ClusterCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the DB cluster was created.\"\n    },\n    \"DBClusterMembers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"DBInstanceIdentifier\": {\n            \"type\": \"string\"\n          },\n          \"IsClusterWriter\": {\n            \"type\": \"boolean\"\n          }\n        }\n      },\n      \"description\": \"The list of instances that make up the DB cluster.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/json-schema/documentdb-openapi-db-cluster-schema.json
tags:
- Amazon Web Services
- AWS
- Database
- Document Database
- DocumentDB
- Managed Database
- MongoDB
- NoSQL
title: DBCluster
---
