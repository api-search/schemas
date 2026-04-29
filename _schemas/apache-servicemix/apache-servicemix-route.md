---
description: Apache Camel route
layout: schema
name: Route
properties_list:
- description: Route identifier
  name: id
  type: string
- description: Route description
  name: description
  type: string
- description: Route status
  name: status
  type: string
- description: Route uptime
  name: uptime
  type: string
- description: Total exchanges processed
  name: exchangesTotal
  type: integer
- description: Failed exchanges count
  name: exchangesFailed
  type: integer
- description: Mean processing time in milliseconds
  name: meanProcessingTime
  type: integer
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-route-schema.json
slug: apache-servicemix-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-route-schema.json\",\n  \"title\": \"Route\",\n  \"description\": \"Apache Camel route\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Route identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Route description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Started\",\n        \"Stopped\",\n        \"Suspended\"\n      ],\n      \"description\": \"Route status\"\n    },\n    \"uptime\": {\n      \"type\": \"string\",\n      \"description\": \"Route uptime\"\n    },\n    \"exchangesTotal\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total exchanges processed\"\n    },\n    \"exchangesFailed\"\
  : {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Failed exchanges count\"\n    },\n    \"meanProcessingTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Mean processing time in milliseconds\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-route-schema.json
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: Route
---
