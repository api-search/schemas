---
description: SnapshotReference schema from Apache Iceberg REST Catalog API
layout: schema
name: SnapshotReference
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: snapshot-id
  type: integer
- description: ''
  name: max-ref-age-ms
  type: integer
- description: ''
  name: max-snapshot-age-ms
  type: integer
- description: ''
  name: min-snapshots-to-keep
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-snapshot-reference-schema.json
slug: rest-catalog-open-api-snapshot-reference
source_filename: rest-catalog-open-api-snapshot-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-snapshot-reference-schema.json\",\n  \"title\": \"SnapshotReference\",\n  \"description\": \"SnapshotReference schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"tag\",\n        \"branch\"\n      ]\n    },\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"max-ref-age-ms\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"max-snapshot-age-ms\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"min-snapshots-to-keep\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"snapshot-id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-snapshot-reference-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SnapshotReference
---
