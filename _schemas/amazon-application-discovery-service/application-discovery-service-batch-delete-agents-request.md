---
description: BatchDeleteAgentsRequest schema from Amazon Application Discovery Service API
layout: schema
name: BatchDeleteAgentsRequest
properties_list:
- description: The list of agents to delete.
  name: deleteAgents
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-batch-delete-agents-request-schema.json
slug: application-discovery-service-batch-delete-agents-request
source_filename: application-discovery-service-batch-delete-agents-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-agents-request-schema.json\",\n  \"title\": \"BatchDeleteAgentsRequest\",\n  \"description\": \"BatchDeleteAgentsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deleteAgents\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"agentId\": {\n            \"type\": \"string\",\n            \"example\": \"d-agent-500123\",\n            \"description\": \"The ID of the agent you want to delete.\"\n          },\n          \"force\": {\n            \"type\": \"boolean\",\n            \"example\": false,\n            \"description\": \"You can use the force parameter to delete agents that do not respond to API\
  \ actions.\"\n          }\n        },\n        \"required\": [\n          \"agentId\"\n        ]\n      },\n      \"description\": \"The list of agents to delete.\"\n    }\n  },\n  \"required\": [\n    \"deleteAgents\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-agents-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: BatchDeleteAgentsRequest
---
