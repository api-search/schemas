---
description: An object that represents the access logging information for a virtual node.
layout: schema
name: AccessLog
properties_list:
- description: ''
  name: file
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-access-log-schema.json
slug: app-mesh-access-log
source_filename: app-mesh-access-log-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"file\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileAccessLog\"\n        },\n        {\n          \"description\": \"The file object to send virtual node access logs to.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the access logging information for a virtual node.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-access-log-schema.json\",\n  \"title\": \"AccessLog\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-access-log-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: AccessLog
---
