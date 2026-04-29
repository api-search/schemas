---
description: RemoveSnapshotRefUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: RemoveSnapshotRefUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: ref-name
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-remove-snapshot-ref-update-schema.json
slug: rest-catalog-open-api-remove-snapshot-ref-update
source_filename: rest-catalog-open-api-remove-snapshot-ref-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-snapshot-ref-update-schema.json\",\n  \"title\": \"RemoveSnapshotRefUpdate\",\n  \"description\": \"RemoveSnapshotRefUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"remove-snapshot-ref\"\n    },\n    \"ref-name\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"ref-name\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-snapshot-ref-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RemoveSnapshotRefUpdate
---
