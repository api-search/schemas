---
description: GetColumnStatisticsForTableResponse schema from Amazon Glue API
layout: schema
name: GetColumnStatisticsForTableResponse
properties_list:
- description: ''
  name: ColumnStatisticsList
  type: object
- description: ''
  name: Errors
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-column-statistics-for-table-response-schema.json
slug: glue-get-column-statistics-for-table-response
source_filename: glue-get-column-statistics-for-table-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-column-statistics-for-table-response-schema.json\",\n  \"title\": \"GetColumnStatisticsForTableResponse\",\n  \"description\": \"GetColumnStatisticsForTableResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ColumnStatisticsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnStatisticsList\"\n        },\n        {\n          \"description\": \"List of ColumnStatistics.\"\n        }\n      ]\n    },\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnErrors\"\n        },\n        {\n          \"description\": \"List of ColumnStatistics that failed to be retrieved.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-column-statistics-for-table-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetColumnStatisticsForTableResponse
---
