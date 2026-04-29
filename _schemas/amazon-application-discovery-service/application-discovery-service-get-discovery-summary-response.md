---
description: GetDiscoverySummaryResponse schema from Amazon Application Discovery Service API
layout: schema
name: GetDiscoverySummaryResponse
properties_list:
- description: The number of servers discovered.
  name: servers
  type: integer
- description: The number of applications discovered.
  name: applications
  type: integer
- description: The number of servers mapped to applications.
  name: serversMappedToApplications
  type: integer
- description: The number of servers mapped to tags.
  name: serversMappedtoTags
  type: integer
- description: The number of servers mapped to applications or tags.
  name: mappedServerCount
  type: integer
- description: The number of servers not mapped to any application.
  name: unmappedServerCount
  type: integer
- description: ''
  name: agentSummary
  type: object
- description: ''
  name: connectorSummary
  type: object
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-get-discovery-summary-response-schema.json
slug: application-discovery-service-get-discovery-summary-response
source_filename: application-discovery-service-get-discovery-summary-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-get-discovery-summary-response-schema.json\",\n  \"title\": \"GetDiscoverySummaryResponse\",\n  \"description\": \"GetDiscoverySummaryResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"servers\": {\n      \"type\": \"integer\",\n      \"example\": 42,\n      \"description\": \"The number of servers discovered.\"\n    },\n    \"applications\": {\n      \"type\": \"integer\",\n      \"example\": 5,\n      \"description\": \"The number of applications discovered.\"\n    },\n    \"serversMappedToApplications\": {\n      \"type\": \"integer\",\n      \"example\": 15,\n      \"description\": \"The number of servers mapped to applications.\"\n    },\n    \"serversMappedtoTags\": {\n      \"type\"\
  : \"integer\",\n      \"example\": 30,\n      \"description\": \"The number of servers mapped to tags.\"\n    },\n    \"mappedServerCount\": {\n      \"type\": \"integer\",\n      \"example\": 15,\n      \"description\": \"The number of servers mapped to applications or tags.\"\n    },\n    \"unmappedServerCount\": {\n      \"type\": \"integer\",\n      \"example\": 27,\n      \"description\": \"The number of servers not mapped to any application.\"\n    },\n    \"agentSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"activeAgents\": {\n          \"type\": \"integer\",\n          \"example\": 3,\n          \"description\": \"Number of active discovery agents.\"\n        },\n        \"healthyAgents\": {\n          \"type\": \"integer\",\n          \"example\": 3,\n          \"description\": \"Number of healthy discovery agents.\"\n        },\n        \"blackListedAgents\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\"\
  : \"Number of blacklisted discovery agents.\"\n        },\n        \"shutdownAgents\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of discovery agents with status SHUTDOWN.\"\n        },\n        \"unhealthyAgents\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of unhealthy discovery agents.\"\n        },\n        \"totalAgents\": {\n          \"type\": \"integer\",\n          \"example\": 3,\n          \"description\": \"Total number of discovery agents.\"\n        },\n        \"unknownAgents\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of unknown discovery agents.\"\n        }\n      }\n    },\n    \"connectorSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"activeConnectors\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of active discovery\
  \ connectors.\"\n        },\n        \"healthyConnectors\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of healthy discovery connectors.\"\n        },\n        \"blackListedConnectors\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of blacklisted discovery connectors.\"\n        },\n        \"shutdownConnectors\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of discovery connectors with status SHUTDOWN.\"\n        },\n        \"unhealthyConnectors\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of unhealthy discovery connectors.\"\n        },\n        \"totalConnectors\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Total number of discovery connectors.\"\n        },\n        \"unknownConnectors\": {\n          \"type\":\
  \ \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of unknown discovery connectors.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-get-discovery-summary-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: GetDiscoverySummaryResponse
---
