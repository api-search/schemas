---
description: CustomerAgentInfo schema from Amazon Application Discovery Service API
layout: schema
name: CustomerAgentInfo
properties_list:
- description: Number of active discovery agents.
  name: activeAgents
  type: integer
- description: Number of healthy discovery agents.
  name: healthyAgents
  type: integer
- description: Number of blacklisted discovery agents.
  name: blackListedAgents
  type: integer
- description: Number of discovery agents with status SHUTDOWN.
  name: shutdownAgents
  type: integer
- description: Number of unhealthy discovery agents.
  name: unhealthyAgents
  type: integer
- description: Total number of discovery agents.
  name: totalAgents
  type: integer
- description: Number of unknown discovery agents.
  name: unknownAgents
  type: integer
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-customer-agent-info-schema.json
slug: application-discovery-service-customer-agent-info
source_filename: application-discovery-service-customer-agent-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-customer-agent-info-schema.json\",\n  \"title\": \"CustomerAgentInfo\",\n  \"description\": \"CustomerAgentInfo schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activeAgents\": {\n      \"type\": \"integer\",\n      \"example\": 3,\n      \"description\": \"Number of active discovery agents.\"\n    },\n    \"healthyAgents\": {\n      \"type\": \"integer\",\n      \"example\": 3,\n      \"description\": \"Number of healthy discovery agents.\"\n    },\n    \"blackListedAgents\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Number of blacklisted discovery agents.\"\n    },\n    \"shutdownAgents\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"\
  description\": \"Number of discovery agents with status SHUTDOWN.\"\n    },\n    \"unhealthyAgents\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Number of unhealthy discovery agents.\"\n    },\n    \"totalAgents\": {\n      \"type\": \"integer\",\n      \"example\": 3,\n      \"description\": \"Total number of discovery agents.\"\n    },\n    \"unknownAgents\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Number of unknown discovery agents.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-customer-agent-info-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: CustomerAgentInfo
---
