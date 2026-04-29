---
description: MLEndpointStatusOutput schema from Neptune
layout: schema
name: MLEndpointStatusOutput
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
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-ml-endpoint-status-output-schema.json
slug: data-ml-endpoint-status-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-ml-endpoint-status-output-schema.json\",\n  \"title\": \"MLEndpointStatusOutput\",\n  \"description\": \"MLEndpointStatusOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"endpoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"arn\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"endpointConfig\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-ml-endpoint-status-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: MLEndpointStatusOutput
---
