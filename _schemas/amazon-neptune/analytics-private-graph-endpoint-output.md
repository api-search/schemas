---
description: PrivateGraphEndpointOutput schema from Neptune
layout: schema
name: PrivateGraphEndpointOutput
properties_list:
- description: ''
  name: vpcId
  type: string
- description: ''
  name: subnetIds
  type: array
- description: ''
  name: status
  type: string
- description: ''
  name: vpcEndpointId
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-private-graph-endpoint-output-schema.json
slug: analytics-private-graph-endpoint-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-private-graph-endpoint-output-schema.json\",\n  \"title\": \"PrivateGraphEndpointOutput\",\n  \"description\": \"PrivateGraphEndpointOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vpcId\": {\n      \"type\": \"string\"\n    },\n    \"subnetIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\",\n        \"AVAILABLE\",\n        \"DELETING\",\n        \"FAILED\"\n      ]\n    },\n    \"vpcEndpointId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-private-graph-endpoint-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: PrivateGraphEndpointOutput
---
