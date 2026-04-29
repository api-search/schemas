---
description: Cluster alert schema from Veritas InfoScale REST API
layout: schema
name: Alert
properties_list:
- description: Alert unique identifier
  name: alertId
  type: string
- description: Alert severity
  name: severity
  type: string
- description: Alert message
  name: message
  type: string
- description: Alert source component
  name: source
  type: string
- description: Alert timestamp
  name: timestamp
  type: string
- description: Whether the alert has been acknowledged
  name: acknowledged
  type: boolean
- description: Related cluster identifier
  name: clusterId
  type: string
provider_name: Veritas InfoScale
provider_slug: veritas-infoscale
schema_file: json-schema/rest-api-alert-schema.json
slug: rest-api-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-alert-schema.json\",\n  \"title\": \"Alert\",\n  \"description\": \"Cluster alert schema from Veritas InfoScale REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alertId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Alert unique identifier\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"critical\", \"warning\", \"info\"],\n      \"description\": \"Alert severity\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Alert message\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Alert source component\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Alert timestamp\"\n\
  \    },\n    \"acknowledged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the alert has been acknowledged\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"description\": \"Related cluster identifier\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/json-schema/rest-api-alert-schema.json
tags:
- Clustering
- Data Management
- Disaster Recovery
- High Availability
- Storage Management
- Virtualization
title: Alert
---
