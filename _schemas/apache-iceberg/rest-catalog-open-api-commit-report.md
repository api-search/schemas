---
description: CommitReport schema from Apache Iceberg REST Catalog API
layout: schema
name: CommitReport
properties_list:
- description: ''
  name: table-name
  type: string
- description: ''
  name: snapshot-id
  type: integer
- description: ''
  name: sequence-number
  type: integer
- description: ''
  name: operation
  type: string
- description: ''
  name: metrics
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-commit-report-schema.json
slug: rest-catalog-open-api-commit-report
source_filename: rest-catalog-open-api-commit-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-commit-report-schema.json\",\n  \"title\": \"CommitReport\",\n  \"description\": \"CommitReport schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"table-name\": {\n      \"type\": \"string\"\n    },\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"sequence-number\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"operation\": {\n      \"type\": \"string\"\n    },\n    \"metrics\": {\n      \"$ref\": \"#/components/schemas/Metrics\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"table-name\",\n    \"snapshot-id\",\n    \"sequence-number\"\
  ,\n    \"operation\",\n    \"metrics\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-commit-report-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CommitReport
---
