---
description: ExportFilter schema from Amazon Application Discovery Service API
layout: schema
name: ExportFilter
properties_list:
- description: A single ExportFilter name. Supported filters — agentIds.
  name: name
  type: string
- description: A single agent ID for a Discovery Agent. An agent ID can be found using the DescribeAgents action.
  name: values
  type: array
- description: Supported condition — EQUALS.
  name: condition
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-export-filter-schema.json
slug: application-discovery-service-export-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-export-filter-schema.json\",\n  \"title\": \"ExportFilter\",\n  \"description\": \"ExportFilter schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"agentIds\",\n      \"description\": \"A single ExportFilter name. Supported filters \\u2014 agentIds.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-agent-500123\"\n      ],\n      \"description\": \"A single agent ID for a Discovery Agent. An agent ID can be found using the DescribeAgents action.\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"example\": \"EQUALS\"\
  ,\n      \"description\": \"Supported condition \\u2014 EQUALS.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"values\",\n    \"condition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-export-filter-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: ExportFilter
---
