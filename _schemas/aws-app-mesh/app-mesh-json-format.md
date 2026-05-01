---
description: JsonFormat schema from AWS App Mesh
layout: schema
name: JsonFormat
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-json-format-schema.json
slug: app-mesh-json-format
source_filename: app-mesh-json-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/JsonKey\"\n          },\n          {\n            \"description\": \"The specified key for the JSON.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/JsonValue\"\n          },\n          {\n            \"description\": \"The specified value for the JSON.\"\n          }\n        ]\n      }\n    },\n    \"required\": [\n      \"key\",\n      \"value\"\n    ],\n    \"description\": \"An object that represents the key value pairs for the JSON.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-json-format-schema.json\",\n  \"title\": \"JsonFormat\",\n  \"description\": \"\
  JsonFormat schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-json-format-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: JsonFormat
---
