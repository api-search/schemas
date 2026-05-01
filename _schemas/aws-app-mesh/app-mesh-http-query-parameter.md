---
description: An object that represents the query parameter in the request.
layout: schema
name: HttpQueryParameter
properties_list:
- description: ''
  name: match
  type: object
- description: ''
  name: name
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-query-parameter-schema.json
slug: app-mesh-http-query-parameter
source_filename: app-mesh-http-query-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"match\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryParameterMatch\"\n        },\n        {\n          \"description\": \"The query parameter to match on.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryParameterName\"\n        },\n        {\n          \"description\": \"A name for the query parameter that will be matched on.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"description\": \"An object that represents the query parameter in the request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-query-parameter-schema.json\",\n  \"title\": \"HttpQueryParameter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-query-parameter-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpQueryParameter
---
