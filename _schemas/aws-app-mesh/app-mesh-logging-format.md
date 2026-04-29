---
description: An object that represents the format for the logs.
layout: schema
name: LoggingFormat
properties_list:
- description: ''
  name: json
  type: object
- description: ''
  name: text
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-logging-format-schema.json
slug: app-mesh-logging-format
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"json\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JsonFormat\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TextFormat\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the format for the logs.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-logging-format-schema.json\",\n  \"title\": \"LoggingFormat\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-logging-format-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: LoggingFormat
---
