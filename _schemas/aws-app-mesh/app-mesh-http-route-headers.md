---
description: HttpRouteHeaders schema from AWS App Mesh
layout: schema
name: HttpRouteHeaders
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-http-route-headers-schema.json
slug: app-mesh-http-route-headers
source_filename: app-mesh-http-route-headers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"invert\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"Specify <code>True</code> to match anything except the match criteria. The default value is <code>False</code>.\"\n          }\n        ]\n      },\n      \"match\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/HeaderMatchMethod\"\n          },\n          {\n            \"description\": \"The <code>HeaderMatchMethod</code> object.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/HeaderName\"\n          },\n          {\n            \"description\": \"A name for the HTTP header in the client request that will be matched on.\"\n          }\n        ]\n      }\n    },\n    \"required\": [\n      \"\
  name\"\n    ],\n    \"description\": \"An object that represents the HTTP header in the request.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-route-headers-schema.json\",\n  \"title\": \"HttpRouteHeaders\",\n  \"description\": \"HttpRouteHeaders schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-http-route-headers-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: HttpRouteHeaders
---
