---
description: CreateGroupResult schema from Amazon X-Ray API
layout: schema
name: CreateGroupResult
properties_list:
- description: ''
  name: Group
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-create-group-result-schema.json
slug: xray-create-group-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Group\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Group\"\n        },\n        {\n          \"description\": \"The group that was created. Contains the name of the group that was created, the Amazon Resource Name (ARN) of the group that was generated based on the group name, the filter expression, and the insight configuration that was assigned to the group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateGroupResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-create-group-result-schema.json\",\n  \"description\": \"CreateGroupResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-create-group-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: CreateGroupResult
---
