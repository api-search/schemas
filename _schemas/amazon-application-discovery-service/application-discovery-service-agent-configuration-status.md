---
description: AgentConfigurationStatus schema from Amazon Application Discovery Service API
layout: schema
name: AgentConfigurationStatus
properties_list:
- description: The agent ID.
  name: agentId
  type: string
- description: Information about the status of the StartDataCollection and StopDataCollection operations.
  name: operationSucceeded
  type: boolean
- description: A description of the operation performed.
  name: description
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-agent-configuration-status-schema.json
slug: application-discovery-service-agent-configuration-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-agent-configuration-status-schema.json\",\n  \"title\": \"AgentConfigurationStatus\",\n  \"description\": \"AgentConfigurationStatus schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentId\": {\n      \"type\": \"string\",\n      \"example\": \"d-agent-500123\",\n      \"description\": \"The agent ID.\"\n    },\n    \"operationSucceeded\": {\n      \"type\": \"boolean\",\n      \"example\": true,\n      \"description\": \"Information about the status of the StartDataCollection and StopDataCollection operations.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Started data collection\",\n      \"description\": \"A description of the operation performed.\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-agent-configuration-status-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: AgentConfigurationStatus
---
