---
description: DescribeAgentsRequest schema from Amazon Application Discovery Service API
layout: schema
name: DescribeAgentsRequest
properties_list:
- description: The agent or the collector IDs for which you want information. If you specify no IDs, the system returns information about all agents/collectors associated with your AWS user account.
  name: agentIds
  type: array
- description: You can filter the request using various logical operators and a key-value format.
  name: filters
  type: array
- description: The total number of agents/collectors to return in a single page of output.
  name: maxResults
  type: integer
- description: Token to retrieve the next set of results.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-agents-request-schema.json
slug: application-discovery-service-describe-agents-request
source_filename: application-discovery-service-describe-agents-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-agents-request-schema.json\",\n  \"title\": \"DescribeAgentsRequest\",\n  \"description\": \"DescribeAgentsRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-agent-500123\"\n      ],\n      \"description\": \"The agent or the collector IDs for which you want information. If you specify no IDs, the system returns information about all agents/collectors associated with your AWS user account.\"\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\":\
  \ {\n            \"type\": \"string\",\n            \"example\": \"hostName\",\n            \"description\": \"The name of the filter.\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"example\": [\n              \"server-01.example.com\"\n            ],\n            \"description\": \"A string value on which to filter.\"\n          },\n          \"condition\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"EQUALS\",\n              \"NOT_EQUALS\",\n              \"CONTAINS\",\n              \"NOT_CONTAINS\"\n            ],\n            \"example\": \"EQUALS\",\n            \"description\": \"A conditional operator. The following operators are valid \\u2014 EQUALS, NOT_EQUALS, CONTAINS, NOT_CONTAINS.\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"values\",\n          \"condition\"\n        ]\n      },\n\
  \      \"description\": \"You can filter the request using various logical operators and a key-value format.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 900,\n      \"example\": 10,\n      \"description\": \"The total number of agents/collectors to return in a single page of output.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"Token to retrieve the next set of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-agents-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DescribeAgentsRequest
---
