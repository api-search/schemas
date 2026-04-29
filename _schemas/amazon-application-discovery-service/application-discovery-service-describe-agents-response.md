---
description: DescribeAgentsResponse schema from Amazon Application Discovery Service API
layout: schema
name: DescribeAgentsResponse
properties_list:
- description: Lists agents or the collectors with status and configuration.
  name: agentsInfo
  type: array
- description: Token to retrieve the next set of results.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-agents-response-schema.json
slug: application-discovery-service-describe-agents-response
source_filename: application-discovery-service-describe-agents-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-agents-response-schema.json\",\n  \"title\": \"DescribeAgentsResponse\",\n  \"description\": \"DescribeAgentsResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentsInfo\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"agentId\": {\n            \"type\": \"string\",\n            \"example\": \"d-agent-500123\",\n            \"description\": \"The agent or collector ID.\"\n          },\n          \"hostName\": {\n            \"type\": \"string\",\n            \"example\": \"server-01.example.com\",\n            \"description\": \"The name of the host where the agent or collector resides.\"\n          },\n\
  \          \"agentNetworkInfoList\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"ipAddress\": {\n                  \"type\": \"string\",\n                  \"description\": \"The IP address for the host where the agent or collector resides.\",\n                  \"example\": \"10.0.0.10\"\n                },\n                \"macAddress\": {\n                  \"type\": \"string\",\n                  \"description\": \"The MAC address for the host where the agent or collector resides.\",\n                  \"example\": \"aa:bb:cc:dd:ee:ff\"\n                }\n              }\n            },\n            \"description\": \"Network details about the host where the agent or collector resides.\"\n          },\n          \"connectorId\": {\n            \"type\": \"string\",\n            \"example\": \"\",\n            \"description\": \"The ID of the connector.\"\n          },\n    \
  \      \"version\": {\n            \"type\": \"string\",\n            \"example\": \"2.0.1\",\n            \"description\": \"The agent or collector version.\"\n          },\n          \"health\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HEALTHY\",\n              \"UNHEALTHY\",\n              \"RUNNING\",\n              \"UNKNOWN\",\n              \"BLACKLISTED\",\n              \"SHUTDOWN\"\n            ],\n            \"example\": \"HEALTHY\",\n            \"description\": \"The health of the agent or collector.\"\n          },\n          \"lastHealthPingTime\": {\n            \"type\": \"string\",\n            \"example\": \"2026-04-19T10:00:00Z\",\n            \"description\": \"Time since agent or collector health was reported.\"\n          },\n          \"collectionStatus\": {\n            \"type\": \"string\",\n            \"example\": \"START_SCHEDULED\",\n            \"description\": \"Status of the collection process for the agent or collector.\"\
  \n          },\n          \"agentType\": {\n            \"type\": \"string\",\n            \"example\": \"AWS_DISCOVERY_AGENT\",\n            \"description\": \"Type of agent.\"\n          },\n          \"registeredTime\": {\n            \"type\": \"string\",\n            \"example\": \"2026-01-01T00:00:00Z\",\n            \"description\": \"Agent's first registration timestamp in UTC.\"\n          }\n        }\n      },\n      \"description\": \"Lists agents or the collectors with status and configuration.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"Token to retrieve the next set of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-agents-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DescribeAgentsResponse
---
