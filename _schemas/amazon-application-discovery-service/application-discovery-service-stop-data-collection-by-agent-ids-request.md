---
description: StopDataCollectionByAgentIdsRequest schema from Amazon Application Discovery Service API
layout: schema
name: StopDataCollectionByAgentIdsRequest
properties_list:
- description: The IDs of the agents from which to stop collecting data.
  name: agentIds
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-stop-data-collection-by-agent-ids-request-schema.json
slug: application-discovery-service-stop-data-collection-by-agent-ids-request
source_filename: application-discovery-service-stop-data-collection-by-agent-ids-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-stop-data-collection-by-agent-ids-request-schema.json\",\n  \"title\": \"StopDataCollectionByAgentIdsRequest\",\n  \"description\": \"StopDataCollectionByAgentIdsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-agent-500123\"\n      ],\n      \"description\": \"The IDs of the agents from which to stop collecting data.\"\n    }\n  },\n  \"required\": [\n    \"agentIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-stop-data-collection-by-agent-ids-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: StopDataCollectionByAgentIdsRequest
---
