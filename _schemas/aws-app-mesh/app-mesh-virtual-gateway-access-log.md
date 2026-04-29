---
description: The access log configuration for a virtual gateway.
layout: schema
name: VirtualGatewayAccessLog
properties_list:
- description: ''
  name: file
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-gateway-access-log-schema.json
slug: app-mesh-virtual-gateway-access-log
source_filename: app-mesh-virtual-gateway-access-log-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"file\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VirtualGatewayFileAccessLog\"\n        },\n        {\n          \"description\": \"The file object to send virtual gateway access logs to.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The access log configuration for a virtual gateway.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-access-log-schema.json\",\n  \"title\": \"VirtualGatewayAccessLog\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-gateway-access-log-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualGatewayAccessLog
---
