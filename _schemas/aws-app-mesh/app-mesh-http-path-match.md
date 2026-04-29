---
description: An object representing the path to match in the request.
layout: schema
name: HttpPathMatch
properties_list:
- description: ''
  name: exact
  type: object
- description: ''
  name: regex
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-path-match-schema.json
slug: app-mesh-http-path-match
source_filename: app-mesh-http-path-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPathExact\"\n        },\n        {\n          \"description\": \"The exact path to match on.\"\n        }\n      ]\n    },\n    \"regex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPathRegex\"\n        },\n        {\n          \"description\": \"The regex used to match the path.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object representing the path to match in the request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-path-match-schema.json\",\n  \"title\": \"HttpPathMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-path-match-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpPathMatch
---
