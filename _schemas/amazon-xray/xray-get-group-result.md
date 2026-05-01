---
description: GetGroupResult schema from Amazon X-Ray API
layout: schema
name: GetGroupResult
properties_list:
- description: ''
  name: Group
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-group-result-schema.json
slug: xray-get-group-result
source_filename: xray-get-group-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Group\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Group\"\n        },\n        {\n          \"description\": \"The group that was requested. Contains the name of the group, the ARN of the group, the filter expression, and the insight configuration assigned to the group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetGroupResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-group-result-schema.json\",\n  \"description\": \"GetGroupResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-group-result-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetGroupResult
---
