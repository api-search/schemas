---
description: GetGroupRequest schema from Amazon X-Ray API
layout: schema
name: GetGroupRequest
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: GroupARN
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-group-request-schema.json
slug: xray-get-group-request
source_filename: xray-get-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"GetGroupRequest\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The case-sensitive name of the group.\"\n        }\n      ]\n    },\n    \"GroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupARN\"\n        },\n        {\n          \"description\": \"The ARN of the group that was generated on creation.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-group-request-schema.json\",\n  \"description\": \"GetGroupRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-group-request-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetGroupRequest
---
