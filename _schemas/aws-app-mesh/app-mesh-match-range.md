---
description: An object that represents the range of values to match on. The first character of the range is included in the range, though the last character is not. For example, if the range specified were 1-100, only values 1-99 would be matched.
layout: schema
name: MatchRange
properties_list:
- description: ''
  name: end
  type: object
- description: ''
  name: start
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-match-range-schema.json
slug: app-mesh-match-range
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"end\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The end of the range.\"\n        }\n      ]\n    },\n    \"start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The start of the range.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"end\",\n    \"start\"\n  ],\n  \"description\": \"An object that represents the range of values to match on. The first character of the range is included in the range, though the last character is not. For example, if the range specified were 1-100, only values 1-99 would be matched.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-match-range-schema.json\",\n  \"\
  title\": \"MatchRange\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-match-range-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: MatchRange
---
