---
description: Usage analytics for Apifuse integrations.
layout: schema
name: Analytics
properties_list:
- description: Total number of tasks executed.
  name: totalTasks
  type: integer
- description: Number of active integrations.
  name: activeIntegrations
  type: integer
- description: Number of active users.
  name: activeUsers
  type: integer
- description: ''
  name: period
  type: object
provider_name: Apifuse
provider_slug: apifuse
schema_file: json-schema/apifuse-analytics-schema.json
slug: apifuse-analytics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/json-schema/apifuse-analytics-schema.json\",\n  \"title\": \"Analytics\",\n  \"description\": \"Usage analytics for Apifuse integrations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalTasks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of tasks executed.\",\n      \"example\": 15420\n    },\n    \"activeIntegrations\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active integrations.\",\n      \"example\": 12\n    },\n    \"activeUsers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active users.\",\n      \"example\": 87\n    },\n    \"period\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"endDate\": {\n      \
  \    \"type\": \"string\",\n          \"format\": \"date\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apifuse/refs/heads/main/json-schema/apifuse-analytics-schema.json
tags:
- Embedded Integrations
- Integration Platform
- Integrations
- iPaaS
- Marketplace
- SaaS
- Workflow Automation
title: Analytics
---
