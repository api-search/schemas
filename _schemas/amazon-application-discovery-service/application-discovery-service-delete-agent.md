---
description: DeleteAgent schema from Amazon Application Discovery Service API
layout: schema
name: DeleteAgent
properties_list:
- description: The ID of the agent you want to delete.
  name: agentId
  type: string
- description: You can use the force parameter to delete agents that do not respond to API actions.
  name: force
  type: boolean
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-delete-agent-schema.json
slug: application-discovery-service-delete-agent
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-delete-agent-schema.json\",\n  \"title\": \"DeleteAgent\",\n  \"description\": \"DeleteAgent schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentId\": {\n      \"type\": \"string\",\n      \"example\": \"d-agent-500123\",\n      \"description\": \"The ID of the agent you want to delete.\"\n    },\n    \"force\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"You can use the force parameter to delete agents that do not respond to API actions.\"\n    }\n  },\n  \"required\": [\n    \"agentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-delete-agent-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DeleteAgent
---
