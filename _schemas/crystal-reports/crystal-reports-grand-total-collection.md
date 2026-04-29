---
description: Collection of grand total summary entries
layout: schema
name: GrandTotalCollection
properties_list:
- description: Array of grand total entries
  name: value
  type: array
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-grand-total-collection-schema.json
slug: crystal-reports-grand-total-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-grand-total-collection-schema.json\",\n  \"title\": \"GrandTotalCollection\",\n  \"description\": \"Collection of grand total summary entries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of grand total entries\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GrandTotal\"\n      },\n      \"example\": [\n        {\n          \"SumOfOrderAmount\": 548290.75,\n          \"CountOfOrders\": 1542,\n          \"AverageOrderAmount\": 355.57\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-grand-total-collection-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: GrandTotalCollection
---
