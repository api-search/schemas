---
description: A CostGuard scan recommendation response containing identified resources, cost analysis, waste metrics, and potential savings for cloud optimization.
layout: schema
name: Finout Scan Recommendation
properties_list:
- description: The ID of this specific request.
  name: requestId
  type: string
- description: The name of the scan.
  name: scanName
  type: string
- description: The last time the scan was run.
  name: scanLastRunTime
  type: string
- description: The sum of resources cost identified by the scan during the analysis days.
  name: scanTotalCost
  type: number
- description: Waste of the scan during the analysis days.
  name: scanTotalWaste
  type: number
- description: Yearly potential savings for the scan based on the scan's total waste.
  name: scanYearlyPotentialSavings
  type: number
- description: Resources identified in the scan with optimization recommendations.
  name: resources
  type: array
provider_name: Finout
provider_slug: finout
schema_file: json-schema/scan-recommendation.json
slug: scan-recommendation
source_filename: scan-recommendation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/finout/blob/main/json-schema/scan-recommendation.json\",\n  \"title\": \"Finout Scan Recommendation\",\n  \"description\": \"A CostGuard scan recommendation response containing identified resources, cost analysis, waste metrics, and potential savings for cloud optimization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of this specific request.\"\n    },\n    \"scanName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the scan.\"\n    },\n    \"scanLastRunTime\": {\n      \"type\": \"string\",\n      \"description\": \"The last time the scan was run.\"\n    },\n    \"scanTotalCost\": {\n      \"type\": \"number\",\n      \"description\": \"The sum of resources cost identified by the scan during the analysis days.\"\n    },\n    \"scanTotalWaste\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"Waste of the scan during the analysis days.\"\n    },\n    \"scanYearlyPotentialSavings\": {\n      \"type\": \"number\",\n      \"description\": \"Yearly potential savings for the scan based on the scan's total waste.\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"Resources identified in the scan with optimization recommendations.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": true\n      }\n    }\n  },\n  \"required\": [\"requestId\", \"scanName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/json-schema/scan-recommendation.json
tags:
- Budgets
- Costs
- FinOps
title: Finout Scan Recommendation
---
