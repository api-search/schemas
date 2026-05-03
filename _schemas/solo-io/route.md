---
description: A route definition within a virtual service or route table, specifying request matchers and the action to take when matched.
layout: schema
name: Solo.io Gloo Gateway Route
properties_list:
- description: Name of the route.
  name: name
  type: string
- description: Request matchers for this route.
  name: matchers
  type: array
- description: Action to take when the route matches.
  name: routeAction
  type: object
- description: Route-level options including transformations and policies.
  name: options
  type: object
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/route.json
slug: route
source_filename: route.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/route.json\",\n  \"title\": \"Solo.io Gloo Gateway Route\",\n  \"description\": \"A route definition within a virtual service or route table, specifying request matchers and the action to take when matched.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the route.\"\n    },\n    \"matchers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"prefix\": {\n            \"type\": \"string\",\n            \"description\": \"URL path prefix to match.\"\n          },\n          \"exact\": {\n            \"type\": \"string\",\n            \"description\": \"Exact URL path to match.\"\n          },\n          \"regex\": {\n            \"type\": \"string\",\n            \"description\": \"\
  Regex pattern for URL path matching.\"\n          },\n          \"headers\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\"\n            },\n            \"description\": \"Header matchers.\"\n          },\n          \"methods\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"HTTP methods to match.\"\n          }\n        }\n      },\n      \"description\": \"Request matchers for this route.\"\n    },\n    \"routeAction\": {\n      \"type\": \"object\",\n      \"description\": \"Action to take when the route matches.\"\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"Route-level options including transformations and policies.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/route.json
tags:
- AI Gateway
- Analytics
- Automation
- Gateways
- Management
- Monetization
- Observability
- Platform
- Resiliency
- Security
- Service Mesh
- Traffic Control
title: Solo.io Gloo Gateway Route
---
