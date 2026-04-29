---
description: The response from the List Agent Pools operation.
layout: schema
name: AgentPoolListResult
properties_list:
- description: The list of agent pools.
  name: value
  type: array
- description: The URL to get the next set of agent pool results.
  name: nextLink
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-kubernetes-service-agent-pool-list-result-schema.json
slug: azure-kubernetes-service-agent-pool-list-result
source_filename: azure-kubernetes-service-agent-pool-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AgentPoolListResult\",\n  \"type\": \"object\",\n  \"description\": \"The response from the List Agent Pools operation.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"The list of agent pools.\"\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to get the next set of agent pool results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-kubernetes-service-agent-pool-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: AgentPoolListResult
---
