---
description: ListAgentStatusesResponse schema from Amazon Connect Service API
layout: schema
name: ListAgentStatusesResponse
properties_list:
- description: ''
  name: AgentStatusSummaryList
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/list-agent-statuses-response-schema.json
slug: list-agent-statuses-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-agent-statuses-response-schema.json\",\n  \"title\": \"ListAgentStatusesResponse\",\n  \"description\": \"ListAgentStatusesResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AgentStatusSummaryList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AgentStatusSummary\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-agent-statuses-response-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ListAgentStatusesResponse
---
