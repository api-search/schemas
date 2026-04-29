---
description: An object representing the query parameter to match.
layout: schema
name: QueryParameterMatch
properties_list:
- description: ''
  name: exact
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-query-parameter-match-schema.json
slug: app-mesh-query-parameter-match
source_filename: app-mesh-query-parameter-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The exact query parameter to match on.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object representing the query parameter to match.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-query-parameter-match-schema.json\",\n  \"title\": \"QueryParameterMatch\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-query-parameter-match-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: QueryParameterMatch
---
