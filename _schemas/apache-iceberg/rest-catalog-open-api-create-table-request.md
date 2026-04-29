---
description: CreateTableRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: CreateTableRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: schema
  type: object
- description: ''
  name: partition-spec
  type: object
- description: ''
  name: write-order
  type: object
- description: ''
  name: stage-create
  type: boolean
- description: ''
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-create-table-request-schema.json
slug: rest-catalog-open-api-create-table-request
source_filename: rest-catalog-open-api-create-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-create-table-request-schema.json\",\n  \"title\": \"CreateTableRequest\",\n  \"description\": \"CreateTableRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"schema\": {\n      \"$ref\": \"#/components/schemas/Schema\"\n    },\n    \"partition-spec\": {\n      \"$ref\": \"#/components/schemas/PartitionSpec\"\n    },\n    \"write-order\": {\n      \"$ref\": \"#/components/schemas/SortOrder\"\n    },\n    \"stage-create\": {\n      \"type\": \"boolean\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n \
  \   \"name\",\n    \"schema\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-create-table-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CreateTableRequest
---
