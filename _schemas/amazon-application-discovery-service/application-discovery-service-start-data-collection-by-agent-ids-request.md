---
description: StartDataCollectionByAgentIdsRequest schema from Amazon Application Discovery Service API
layout: schema
name: StartDataCollectionByAgentIdsRequest
properties_list:
- description: 'The IDs of the agents from which to start collecting data. If you send a request to an agent that you do not have permission to contact, according to your AWS account''s permission settings, the agent '
  name: agentIds
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-start-data-collection-by-agent-ids-request-schema.json
slug: application-discovery-service-start-data-collection-by-agent-ids-request
source_filename: application-discovery-service-start-data-collection-by-agent-ids-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-data-collection-by-agent-ids-request-schema.json\",\n  \"title\": \"StartDataCollectionByAgentIdsRequest\",\n  \"description\": \"StartDataCollectionByAgentIdsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-agent-500123\"\n      ],\n      \"description\": \"The IDs of the agents from which to start collecting data. If you send a request to an agent that you do not have permission to contact, according to your AWS account's permission settings, the agent is not included in the list of agents that are started.\"\n    }\n  },\n  \"required\": [\n\
  \    \"agentIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-data-collection-by-agent-ids-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: StartDataCollectionByAgentIdsRequest
---
