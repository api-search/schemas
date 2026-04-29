---
description: ViewMetadata schema from Apache Iceberg REST Catalog API
layout: schema
name: ViewMetadata
properties_list:
- description: ''
  name: view-uuid
  type: string
- description: ''
  name: format-version
  type: integer
- description: ''
  name: location
  type: string
- description: ''
  name: current-version-id
  type: integer
- description: ''
  name: versions
  type: array
- description: ''
  name: version-log
  type: array
- description: ''
  name: schemas
  type: array
- description: ''
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-view-metadata-schema.json
slug: rest-catalog-open-api-view-metadata
source_filename: rest-catalog-open-api-view-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-view-metadata-schema.json\",\n  \"title\": \"ViewMetadata\",\n  \"description\": \"ViewMetadata schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"view-uuid\": {\n      \"type\": \"string\"\n    },\n    \"format-version\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 1\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"current-version-id\": {\n      \"type\": \"integer\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ViewVersion\"\n      }\n    },\n    \"version-log\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ViewHistoryEntry\"\n      }\n    },\n    \"schemas\":\
  \ {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Schema\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"view-uuid\",\n    \"format-version\",\n    \"location\",\n    \"current-version-id\",\n    \"versions\",\n    \"version-log\",\n    \"schemas\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-view-metadata-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ViewMetadata
---
