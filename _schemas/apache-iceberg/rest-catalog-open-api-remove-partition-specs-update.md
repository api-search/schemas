---
description: RemovePartitionSpecsUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: RemovePartitionSpecsUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: spec-ids
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-remove-partition-specs-update-schema.json
slug: rest-catalog-open-api-remove-partition-specs-update
source_filename: rest-catalog-open-api-remove-partition-specs-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-partition-specs-update-schema.json\",\n  \"title\": \"RemovePartitionSpecsUpdate\",\n  \"description\": \"RemovePartitionSpecsUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"remove-partition-specs\"\n    },\n    \"spec-ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"required\": [\n    \"spec-ids\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-partition-specs-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RemovePartitionSpecsUpdate
---
