---
description: RemoveSnapshotsUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: RemoveSnapshotsUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: snapshot-ids
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-remove-snapshots-update-schema.json
slug: rest-catalog-open-api-remove-snapshots-update
source_filename: rest-catalog-open-api-remove-snapshots-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-snapshots-update-schema.json\",\n  \"title\": \"RemoveSnapshotsUpdate\",\n  \"description\": \"RemoveSnapshotsUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"remove-snapshots\"\n    },\n    \"snapshot-ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      }\n    }\n  },\n  \"required\": [\n    \"snapshot-ids\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-snapshots-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RemoveSnapshotsUpdate
---
