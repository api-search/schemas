---
description: EndpointStatusResponse schema from Neptune
layout: schema
name: EndpointStatusResponse
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: endpoint
  type: object
- description: ''
  name: endpointConfig
  type: object
- description: ''
  name: outputLocation
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/ml-endpoint-status-response-schema.json
slug: ml-endpoint-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-endpoint-status-response-schema.json\",\n  \"title\": \"EndpointStatusResponse\",\n  \"description\": \"EndpointStatusResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"endpoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"arn\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"endpointConfig\": {\n      \"type\": \"object\"\n    },\n    \"outputLocation\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-endpoint-status-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: EndpointStatusResponse
---
