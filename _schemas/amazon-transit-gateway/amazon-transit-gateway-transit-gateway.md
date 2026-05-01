---
description: ''
layout: schema
name: TransitGateway
properties_list:
- description: The ID of the transit gateway.
  name: TransitGatewayId
  type: string
- description: The Amazon Resource Name (ARN) of the transit gateway.
  name: TransitGatewayArn
  type: string
- description: ''
  name: State
  type: string
- description: ''
  name: OwnerId
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: CreationTime
  type: string
provider_name: Amazon Transit Gateway
provider_slug: amazon-transit-gateway
schema_file: json-schema/amazon-transit-gateway-transit-gateway-schema.json
slug: amazon-transit-gateway-transit-gateway
source_filename: amazon-transit-gateway-transit-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransitGatewayId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the transit gateway.\"\n    },\n    \"TransitGatewayArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the transit gateway.\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"available\",\n        \"modifying\",\n        \"deleting\",\n        \"deleted\"\n      ]\n    },\n    \"OwnerId\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TransitGateway\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-transit-gateway/refs/heads/main/json-schema/amazon-transit-gateway-transit-gateway-schema.json
tags:
- Cloud Networking
- Network Hub
- Networking
- Transit Gateway
- VPC
title: TransitGateway
---
