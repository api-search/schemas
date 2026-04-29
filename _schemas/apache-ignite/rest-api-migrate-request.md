---
description: Migrate nodes to new cluster.
layout: schema
name: MigrateRequest
properties_list:
- description: Names of the CMG node names.
  name: cmgNodes
  type: array
- description: Names of the Metastorage node names.
  name: metaStorageNodes
  type: array
- description: Ignite version.
  name: version
  type: string
- description: ID of the cluster.
  name: clusterId
  type: string
- description: Name of the cluster.
  name: clusterName
  type: string
- description: IDs the cluster had before. If CMG/Metastorage group were never repaired, this is null.
  name: formerClusterIds
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-migrate-request-schema.json
slug: rest-api-migrate-request
source_filename: rest-api-migrate-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-migrate-request-schema.json\",\n  \"title\": \"MigrateRequest\",\n  \"description\": \"Migrate nodes to new cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cmgNodes\": {\n      \"type\": \"array\",\n      \"description\": \"Names of the CMG node names.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"metaStorageNodes\": {\n      \"type\": \"array\",\n      \"description\": \"Names of the Metastorage node names.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Ignite version.\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the cluster.\",\n      \"format\": \"uuid\"\n    },\n    \"clusterName\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Name of the cluster.\"\n    },\n    \"formerClusterIds\": {\n      \"type\": \"array\",\n      \"description\": \"IDs the cluster had before. If CMG/Metastorage group were never repaired, this is null.\",\n      \"nullable\": true,\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-migrate-request-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: MigrateRequest
---
