---
description: Contains the details of a Neptune DB cluster snapshot.
layout: schema
name: DBClusterSnapshot
properties_list:
- description: The identifier of the cluster snapshot.
  name: DBClusterSnapshotIdentifier
  type: string
- description: The cluster identifier of the source cluster.
  name: DBClusterIdentifier
  type: string
- description: ''
  name: SnapshotCreateTime
  type: string
- description: ''
  name: Engine
  type: string
- description: ''
  name: EngineVersion
  type: string
- description: The status of the snapshot.
  name: Status
  type: string
- description: ''
  name: AllocatedStorage
  type: integer
- description: ''
  name: VpcId
  type: string
- description: ''
  name: Port
  type: integer
- description: ''
  name: StorageEncrypted
  type: boolean
- description: ''
  name: KmsKeyId
  type: string
- description: ''
  name: DBClusterSnapshotArn
  type: string
- description: The type of the snapshot (manual or automated).
  name: SnapshotType
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-db-cluster-snapshot-schema.json
slug: management-db-cluster-snapshot
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-cluster-snapshot-schema.json\",\n  \"title\": \"DBClusterSnapshot\",\n  \"description\": \"Contains the details of a Neptune DB cluster snapshot.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBClusterSnapshotIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the cluster snapshot.\"\n    },\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster identifier of the source cluster.\"\n    },\n    \"SnapshotCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Engine\": {\n      \"type\": \"string\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the snapshot.\"\
  \n    },\n    \"AllocatedStorage\": {\n      \"type\": \"integer\"\n    },\n    \"VpcId\": {\n      \"type\": \"string\"\n    },\n    \"Port\": {\n      \"type\": \"integer\"\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\"\n    },\n    \"DBClusterSnapshotArn\": {\n      \"type\": \"string\"\n    },\n    \"SnapshotType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the snapshot (manual or automated).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-cluster-snapshot-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DBClusterSnapshot
---
