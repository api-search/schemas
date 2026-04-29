---
description: Dashboard schema from openapi
layout: schema
name: Dashboard
properties_list:
- description: ''
  name: DashboardId
  type: string
- description: ''
  name: Arn
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: Version
  type: object
- description: ''
  name: CreatedTime
  type: string
- description: ''
  name: LastPublishedTime
  type: string
- description: ''
  name: LastUpdatedTime
  type: string
provider_name: Amazon QuickSight
provider_slug: amazon-quicksight
schema_file: json-schema/amazon-quicksight-openapi-dashboard-schema.json
slug: amazon-quicksight-openapi-dashboard
source_filename: amazon-quicksight-openapi-dashboard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-quicksight/refs/heads/main/json-schema/amazon-quicksight-openapi-dashboard-schema.json\",\n  \"title\": \"Dashboard\",\n  \"description\": \"Dashboard schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashboardId\": {\n      \"type\": \"string\"\n    },\n    \"Arn\": {\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Version\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"VersionNumber\": {\n          \"type\": \"integer\"\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"CREATION_IN_PROGRESS\",\n            \"CREATION_SUCCESSFUL\",\n            \"CREATION_FAILED\",\n            \"UPDATE_IN_PROGRESS\",\n            \"UPDATE_SUCCESSFUL\",\n            \"UPDATE_FAILED\"\n          ]\n       \
  \ },\n        \"CreatedTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"CreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastPublishedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-quicksight/refs/heads/main/json-schema/amazon-quicksight-openapi-dashboard-schema.json
tags:
- Analytics
- AWS
- BI
- Business Intelligence
- Dashboards
- Machine Learning
- Reporting
- Visualization
title: Dashboard
---
