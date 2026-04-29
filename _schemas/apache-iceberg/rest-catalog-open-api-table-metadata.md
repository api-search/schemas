---
description: TableMetadata schema from Apache Iceberg REST Catalog API
layout: schema
name: TableMetadata
properties_list:
- description: ''
  name: format-version
  type: integer
- description: ''
  name: table-uuid
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: last-updated-ms
  type: integer
- description: A long higher than all assigned row IDs; the next snapshot's first-row-id.
  name: next-row-id
  type: integer
- description: ''
  name: properties
  type: object
- description: ''
  name: schemas
  type: array
- description: ''
  name: current-schema-id
  type: integer
- description: ''
  name: last-column-id
  type: integer
- description: ''
  name: partition-specs
  type: array
- description: ''
  name: default-spec-id
  type: integer
- description: ''
  name: last-partition-id
  type: integer
- description: ''
  name: sort-orders
  type: array
- description: ''
  name: default-sort-order-id
  type: integer
- description: ''
  name: encryption-keys
  type: array
- description: ''
  name: snapshots
  type: array
- description: ''
  name: refs
  type: object
- description: ''
  name: current-snapshot-id
  type: integer
- description: ''
  name: last-sequence-number
  type: integer
- description: ''
  name: snapshot-log
  type: object
- description: ''
  name: metadata-log
  type: object
- description: ''
  name: statistics
  type: array
- description: ''
  name: partition-statistics
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-table-metadata-schema.json
slug: rest-catalog-open-api-table-metadata
source_filename: rest-catalog-open-api-table-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-table-metadata-schema.json\",\n  \"title\": \"TableMetadata\",\n  \"description\": \"TableMetadata schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"format-version\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 3\n    },\n    \"table-uuid\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"last-updated-ms\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"next-row-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"A long higher than all assigned row IDs; the next snapshot's first-row-id.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Schema\"\n      }\n    },\n    \"current-schema-id\": {\n      \"type\": \"integer\"\n    },\n    \"last-column-id\": {\n      \"type\": \"integer\"\n    },\n    \"partition-specs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PartitionSpec\"\n      }\n    },\n    \"default-spec-id\": {\n      \"type\": \"integer\"\n    },\n    \"last-partition-id\": {\n      \"type\": \"integer\"\n    },\n    \"sort-orders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SortOrder\"\n      }\n    },\n    \"default-sort-order-id\": {\n      \"type\": \"integer\"\n    },\n    \"encryption-keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EncryptedKey\"\n      }\n    },\n    \"snapshots\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Snapshot\"\n      }\n    },\n    \"refs\": {\n      \"$ref\": \"#/components/schemas/SnapshotReferences\"\n    },\n    \"current-snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"last-sequence-number\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"snapshot-log\": {\n      \"$ref\": \"#/components/schemas/SnapshotLog\"\n    },\n    \"metadata-log\": {\n      \"$ref\": \"#/components/schemas/MetadataLog\"\n    },\n    \"statistics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StatisticsFile\"\n      }\n    },\n    \"partition-statistics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PartitionStatisticsFile\"\n      }\n    }\n  },\n  \"required\": [\n    \"format-version\",\n    \"table-uuid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-table-metadata-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: TableMetadata
---
