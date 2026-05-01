---
description: RestoreDBClusterFromSnapshotRequest schema from Neptune
layout: schema
name: RestoreDBClusterFromSnapshotRequest
properties_list:
- description: The name of the new DB cluster.
  name: DBClusterIdentifier
  type: string
- description: The identifier of the snapshot to restore from.
  name: SnapshotIdentifier
  type: string
- description: The database engine to use.
  name: Engine
  type: string
- description: ''
  name: EngineVersion
  type: string
- description: ''
  name: Port
  type: integer
- description: ''
  name: DBSubnetGroupName
  type: string
- description: ''
  name: VpcSecurityGroupIds
  type: array
- description: ''
  name: DeletionProtection
  type: boolean
- description: ''
  name: IAMDatabaseAuthenticationEnabled
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-restore-db-cluster-from-snapshot-request-schema.json
slug: management-restore-db-cluster-from-snapshot-request
source_filename: management-restore-db-cluster-from-snapshot-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-restore-db-cluster-from-snapshot-request-schema.json\",\n  \"title\": \"RestoreDBClusterFromSnapshotRequest\",\n  \"description\": \"RestoreDBClusterFromSnapshotRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the new DB cluster.\"\n    },\n    \"SnapshotIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the snapshot to restore from.\"\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine to use.\",\n      \"default\": \"neptune\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\"\n    },\n    \"Port\": {\n      \"type\": \"integer\"\n    },\n    \"DBSubnetGroupName\": {\n\
  \      \"type\": \"string\"\n    },\n    \"VpcSecurityGroupIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"DeletionProtection\": {\n      \"type\": \"boolean\"\n    },\n    \"IAMDatabaseAuthenticationEnabled\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"DBClusterIdentifier\",\n    \"SnapshotIdentifier\",\n    \"Engine\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-restore-db-cluster-from-snapshot-request-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: RestoreDBClusterFromSnapshotRequest
---
