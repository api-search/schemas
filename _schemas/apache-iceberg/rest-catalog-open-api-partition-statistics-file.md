---
description: PartitionStatisticsFile schema from Apache Iceberg REST Catalog API
layout: schema
name: PartitionStatisticsFile
properties_list:
- description: ''
  name: snapshot-id
  type: integer
- description: ''
  name: statistics-path
  type: string
- description: ''
  name: file-size-in-bytes
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-partition-statistics-file-schema.json
slug: rest-catalog-open-api-partition-statistics-file
source_filename: rest-catalog-open-api-partition-statistics-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-partition-statistics-file-schema.json\",\n  \"title\": \"PartitionStatisticsFile\",\n  \"description\": \"PartitionStatisticsFile schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"statistics-path\": {\n      \"type\": \"string\"\n    },\n    \"file-size-in-bytes\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\": [\n    \"snapshot-id\",\n    \"statistics-path\",\n    \"file-size-in-bytes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-partition-statistics-file-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: PartitionStatisticsFile
---
