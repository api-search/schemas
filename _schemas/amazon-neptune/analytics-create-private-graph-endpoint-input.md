---
description: CreatePrivateGraphEndpointInput schema from Neptune
layout: schema
name: CreatePrivateGraphEndpointInput
properties_list:
- description: The VPC ID for the private endpoint.
  name: vpcId
  type: string
- description: The subnet IDs for the private endpoint.
  name: subnetIds
  type: array
- description: The security group IDs for the private endpoint.
  name: vpcSecurityGroupIds
  type: array
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-create-private-graph-endpoint-input-schema.json
slug: analytics-create-private-graph-endpoint-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-create-private-graph-endpoint-input-schema.json\",\n  \"title\": \"CreatePrivateGraphEndpointInput\",\n  \"description\": \"CreatePrivateGraphEndpointInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The VPC ID for the private endpoint.\"\n    },\n    \"subnetIds\": {\n      \"type\": \"array\",\n      \"description\": \"The subnet IDs for the private endpoint.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"vpcSecurityGroupIds\": {\n      \"type\": \"array\",\n      \"description\": \"The security group IDs for the private endpoint.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-create-private-graph-endpoint-input-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreatePrivateGraphEndpointInput
---
