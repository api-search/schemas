---
description: ''
layout: schema
name: EndpointConfiguration
properties_list:
- description: A list of endpoint types of an API or its custom domain name.
  name: types
  type: array
- description: A list of VPC endpoint IDs of an API against which to create Route53 ALIASes.
  name: vpcEndpointIds
  type: array
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-endpointconfiguration-schema.json
slug: amazon-api-gateway-endpointconfiguration
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"EndpointConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"A list of endpoint types of an API or its custom domain name.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"REGIONAL\",\n          \"EDGE\",\n          \"PRIVATE\"\n        ]\n      }\n    },\n    \"vpcEndpointIds\": {\n      \"type\": \"array\",\n      \"description\": \"A list of VPC endpoint IDs of an API against which to create Route53 ALIASes.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-endpointconfiguration-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: EndpointConfiguration
---
