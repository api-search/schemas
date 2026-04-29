---
description: An object that represents logging information.
layout: schema
name: VirtualGatewayLogging
properties_list:
- description: ''
  name: accessLog
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-logging-schema.json
slug: app-mesh-virtual-gateway-logging
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessLog\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayAccessLog\"\n        },\n        {\n          \"description\": \"The access log configuration.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents logging information.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-logging-schema.json\",\n  \"title\": \"VirtualGatewayLogging\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-logging-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayLogging
---
