---
description: UpdateGroupResult schema from Amazon X-Ray API
layout: schema
name: UpdateGroupResult
properties_list:
- description: ''
  name: Group
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-update-group-result-schema.json
slug: xray-update-group-result
source_filename: xray-update-group-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Group\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Group\"\n        },\n        {\n          \"description\": \"The group that was updated. Contains the name of the group that was updated, the ARN of the group that was updated, the updated filter expression, and the updated insight configuration assigned to the group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateGroupResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-update-group-result-schema.json\",\n  \"description\": \"UpdateGroupResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-update-group-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: UpdateGroupResult
---
