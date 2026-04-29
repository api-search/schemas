---
description: BatchDeleteAgentError schema from Amazon Application Discovery Service API
layout: schema
name: BatchDeleteAgentError
properties_list:
- description: The ID of the agent that failed to delete.
  name: agentId
  type: string
- description: The type of error that occurred.
  name: errorCode
  type: string
- description: The text of the error message.
  name: errorMessage
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-batch-delete-agent-error-schema.json
slug: application-discovery-service-batch-delete-agent-error
source_filename: application-discovery-service-batch-delete-agent-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-agent-error-schema.json\",\n  \"title\": \"BatchDeleteAgentError\",\n  \"description\": \"BatchDeleteAgentError schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentId\": {\n      \"type\": \"string\",\n      \"example\": \"d-agent-500123\",\n      \"description\": \"The ID of the agent that failed to delete.\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"example\": \"NOT_FOUND\",\n      \"description\": \"The type of error that occurred.\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"example\": \"Agent not found\",\n      \"description\": \"The text of the error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-agent-error-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: BatchDeleteAgentError
---
