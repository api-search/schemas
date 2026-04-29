---
description: An object that represents the logging information for a virtual node.
layout: schema
name: Logging
properties_list:
- description: ''
  name: accessLog
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-logging-schema.json
slug: app-mesh-logging
source_filename: app-mesh-logging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessLog\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessLog\"\n        },\n        {\n          \"description\": \"The access log configuration for a virtual node.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the logging information for a virtual node.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-logging-schema.json\",\n  \"title\": \"Logging\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-logging-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: Logging
---
