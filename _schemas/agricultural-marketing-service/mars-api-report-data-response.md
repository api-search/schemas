---
description: Response containing detailed report data.
layout: schema
name: Report Data Response
properties_list:
- description: ''
  name: results
  type: array
- description: ''
  name: stats
  type: object
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
schema_file: json-schema/mars-api-report-data-response-schema.json
slug: mars-api-report-data-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-report-data-response-schema.json\",\n  \"title\": \"Report Data Response\",\n  \"description\": \"Response containing detailed report data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ReportData\"\n      }\n    },\n    \"stats\": {\n      \"$ref\": \"#/components/schemas/PaginationStats\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-report-data-response-schema.json
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
title: Report Data Response
---
