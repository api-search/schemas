---
description: DescribeVirtualGatewayOutput schema from AWS App Mesh
layout: schema
name: DescribeVirtualGatewayOutput
properties_list:
- description: ''
  name: virtualGateway
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-describe-virtual-gateway-output-schema.json
slug: app-mesh-describe-virtual-gateway-output
source_filename: app-mesh-describe-virtual-gateway-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"virtualGateway\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayData\"\n        },\n        {\n          \"description\": \"The full description of your virtual gateway.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualGateway\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-describe-virtual-gateway-output-schema.json\",\n  \"title\": \"DescribeVirtualGatewayOutput\",\n  \"description\": \"DescribeVirtualGatewayOutput schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-describe-virtual-gateway-output-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: DescribeVirtualGatewayOutput
---
