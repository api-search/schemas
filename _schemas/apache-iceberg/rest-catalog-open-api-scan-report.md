---
description: ScanReport schema from Apache Iceberg REST Catalog API
layout: schema
name: ScanReport
properties_list:
- description: ''
  name: table-name
  type: string
- description: ''
  name: snapshot-id
  type: integer
- description: ''
  name: filter
  type: object
- description: ''
  name: schema-id
  type: integer
- description: ''
  name: projected-field-ids
  type: array
- description: ''
  name: projected-field-names
  type: array
- description: ''
  name: metrics
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-scan-report-schema.json
slug: rest-catalog-open-api-scan-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-scan-report-schema.json\",\n  \"title\": \"ScanReport\",\n  \"description\": \"ScanReport schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"table-name\": {\n      \"type\": \"string\"\n    },\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"filter\": {\n      \"$ref\": \"#/components/schemas/Expression\"\n    },\n    \"schema-id\": {\n      \"type\": \"integer\"\n    },\n    \"projected-field-ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"projected-field-names\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"metrics\": {\n      \"$ref\": \"#/components/schemas/Metrics\"\
  \n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"table-name\",\n    \"snapshot-id\",\n    \"filter\",\n    \"schema-id\",\n    \"projected-field-ids\",\n    \"projected-field-names\",\n    \"metrics\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-scan-report-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ScanReport
---
