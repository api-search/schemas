---
description: Represents a copy of an entire cluster.
layout: schema
name: Snapshot
properties_list:
- description: The ARN of the snapshot.
  name: ARN
  type: string
- description: The configuration of the cluster from which the snapshot was taken.
  name: ClusterConfiguration
  type: object
- description: The ID of the KMS key used to encrypt the snapshot.
  name: KmsKeyId
  type: string
- description: The name of the snapshot.
  name: Name
  type: string
- description: The status of the snapshot.
  name: Status
  type: string
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-snapshot-schema.json
slug: memorydb-api-snapshot
source_filename: memorydb-api-snapshot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-snapshot-schema.json\",\n  \"title\": \"Snapshot\",\n  \"description\": \"Represents a copy of an entire cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"description\": \"The ARN of the snapshot.\",\n      \"type\": \"string\"\n    },\n    \"ClusterConfiguration\": {\n      \"description\": \"The configuration of the cluster from which the snapshot was taken.\",\n      \"type\": \"object\"\n    },\n    \"KmsKeyId\": {\n      \"description\": \"The ID of the KMS key used to encrypt the snapshot.\",\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"description\": \"The name of the snapshot.\",\n      \"type\": \"string\"\n    },\n    \"Status\": {\n      \"description\": \"The status of the snapshot.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-snapshot-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Snapshot
---
