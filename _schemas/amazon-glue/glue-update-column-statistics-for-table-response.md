---
description: UpdateColumnStatisticsForTableResponse schema from Amazon Glue API
layout: schema
name: UpdateColumnStatisticsForTableResponse
properties_list:
- description: ''
  name: Errors
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-column-statistics-for-table-response-schema.json
slug: glue-update-column-statistics-for-table-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-column-statistics-for-table-response-schema.json\",\n  \"title\": \"UpdateColumnStatisticsForTableResponse\",\n  \"description\": \"UpdateColumnStatisticsForTableResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnStatisticsErrors\"\n        },\n        {\n          \"description\": \"List of ColumnStatisticsErrors.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-column-statistics-for-table-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateColumnStatisticsForTableResponse
---
