---
description: MapType schema from Apache Iceberg REST Catalog API
layout: schema
name: MapType
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: key-id
  type: integer
- description: ''
  name: key
  type: object
- description: ''
  name: value-id
  type: integer
- description: ''
  name: value
  type: object
- description: ''
  name: value-required
  type: boolean
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-map-type-schema.json
slug: rest-catalog-open-api-map-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-map-type-schema.json\",\n  \"title\": \"MapType\",\n  \"description\": \"MapType schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"map\"\n    },\n    \"key-id\": {\n      \"type\": \"integer\"\n    },\n    \"key\": {\n      \"$ref\": \"#/components/schemas/Type\"\n    },\n    \"value-id\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"$ref\": \"#/components/schemas/Type\"\n    },\n    \"value-required\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"key-id\",\n    \"key\",\n    \"value-id\",\n    \"value\",\n    \"value-required\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-map-type-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: MapType
---
