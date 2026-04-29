---
description: StartDataCollectionByAgentIdsResponse schema from Amazon Application Discovery Service API
layout: schema
name: StartDataCollectionByAgentIdsResponse
properties_list:
- description: Information about agents that were instructed to start collecting data. Information includes the agent ID, a description of the operation performed, and whether the agent configuration was updated suc
  name: agentsConfigurationStatus
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-start-data-collection-by-agent-ids-response-schema.json
slug: application-discovery-service-start-data-collection-by-agent-ids-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-data-collection-by-agent-ids-response-schema.json\",\n  \"title\": \"StartDataCollectionByAgentIdsResponse\",\n  \"description\": \"StartDataCollectionByAgentIdsResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentsConfigurationStatus\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"agentId\": {\n            \"type\": \"string\",\n            \"example\": \"d-agent-500123\",\n            \"description\": \"The agent ID.\"\n          },\n          \"operationSucceeded\": {\n            \"type\": \"boolean\",\n            \"example\": true,\n            \"description\": \"Information about the status of the\
  \ StartDataCollection and StopDataCollection operations.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Started data collection\",\n            \"description\": \"A description of the operation performed.\"\n          }\n        }\n      },\n      \"description\": \"Information about agents that were instructed to start collecting data. Information includes the agent ID, a description of the operation performed, and whether the agent configuration was updated successfully.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-data-collection-by-agent-ids-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: StartDataCollectionByAgentIdsResponse
---
