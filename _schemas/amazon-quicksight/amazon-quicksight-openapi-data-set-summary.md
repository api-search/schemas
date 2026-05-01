---
description: DataSetSummary schema from openapi
layout: schema
name: DataSetSummary
properties_list:
- description: ''
  name: Arn
  type: string
- description: ''
  name: DataSetId
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: CreatedTime
  type: string
- description: ''
  name: LastUpdatedTime
  type: string
- description: ''
  name: ImportMode
  type: string
provider_name: Amazon QuickSight
provider_slug: amazon-quicksight
schema_file: json-schema/amazon-quicksight-openapi-data-set-summary-schema.json
slug: amazon-quicksight-openapi-data-set-summary
source_filename: amazon-quicksight-openapi-data-set-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-quicksight/refs/heads/main/json-schema/amazon-quicksight-openapi-data-set-summary-schema.json\",\n  \"title\": \"DataSetSummary\",\n  \"description\": \"DataSetSummary schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\"\n    },\n    \"DataSetId\": {\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"CreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"ImportMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SPICE\",\n        \"DIRECT_QUERY\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-quicksight/refs/heads/main/json-schema/amazon-quicksight-openapi-data-set-summary-schema.json
tags:
- Analytics
- BI
- Business Intelligence
- Dashboards
- Machine Learning
- Reporting
- Visualization
title: DataSetSummary
---
