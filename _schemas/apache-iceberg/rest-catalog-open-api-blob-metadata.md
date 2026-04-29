---
description: BlobMetadata schema from Apache Iceberg REST Catalog API
layout: schema
name: BlobMetadata
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: snapshot-id
  type: integer
- description: ''
  name: sequence-number
  type: integer
- description: ''
  name: fields
  type: array
- description: ''
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-blob-metadata-schema.json
slug: rest-catalog-open-api-blob-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-blob-metadata-schema.json\",\n  \"title\": \"BlobMetadata\",\n  \"description\": \"BlobMetadata schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"sequence-number\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"snapshot-id\",\n    \"sequence-number\",\n    \"fields\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-blob-metadata-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: BlobMetadata
---
