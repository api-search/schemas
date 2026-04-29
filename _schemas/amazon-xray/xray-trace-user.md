---
description: Information about a user recorded in segment documents.
layout: schema
name: TraceUser
properties_list:
- description: ''
  name: UserName
  type: object
- description: ''
  name: ServiceIds
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-trace-user-schema.json
slug: xray-trace-user
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The user's name.\"\n        }\n      ]\n    },\n    \"ServiceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceIds\"\n        },\n        {\n          \"description\": \"Services that the user's request hit.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about a user recorded in segment documents.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TraceUser\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-trace-user-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-trace-user-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: TraceUser
---
