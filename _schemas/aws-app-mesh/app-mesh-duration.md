---
description: An object that represents a duration of time.
layout: schema
name: Duration
properties_list:
- description: ''
  name: unit
  type: object
- description: ''
  name: value
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-duration-schema.json
slug: app-mesh-duration
source_filename: app-mesh-duration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationUnit\"\n        },\n        {\n          \"description\": \"A unit of time.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationValue\"\n        },\n        {\n          \"description\": \"A number of time units.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents a duration of time.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-duration-schema.json\",\n  \"title\": \"Duration\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-duration-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: Duration
---
