---
description: ViewVersion schema from Apache Iceberg REST Catalog API
layout: schema
name: ViewVersion
properties_list:
- description: ''
  name: version-id
  type: integer
- description: ''
  name: timestamp-ms
  type: integer
- description: Schema ID to set as current, or -1 to set last added schema
  name: schema-id
  type: integer
- description: ''
  name: summary
  type: object
- description: ''
  name: representations
  type: array
- description: ''
  name: default-catalog
  type: string
- description: ''
  name: default-namespace
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-view-version-schema.json
slug: rest-catalog-open-api-view-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-view-version-schema.json\",\n  \"title\": \"ViewVersion\",\n  \"description\": \"ViewVersion schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version-id\": {\n      \"type\": \"integer\"\n    },\n    \"timestamp-ms\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"schema-id\": {\n      \"type\": \"integer\",\n      \"description\": \"Schema ID to set as current, or -1 to set last added schema\"\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"representations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ViewRepresentation\"\n      }\n    },\n    \"default-catalog\"\
  : {\n      \"type\": \"string\"\n    },\n    \"default-namespace\": {\n      \"$ref\": \"#/components/schemas/Namespace\"\n    }\n  },\n  \"required\": [\n    \"version-id\",\n    \"timestamp-ms\",\n    \"schema-id\",\n    \"summary\",\n    \"representations\",\n    \"default-namespace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-view-version-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ViewVersion
---
