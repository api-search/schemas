---
description: UntagResourceRequest schema from Amazon X-Ray API
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-untag-resource-request-schema.json
slug: xray-untag-resource-request
source_filename: xray-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceARN\",\n    \"TagKeys\"\n  ],\n  \"title\": \"UntagResourceRequest\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Number (ARN) of an X-Ray group or sampling rule.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"Keys for one or more tags that you want to remove from an X-Ray group or sampling rule.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-untag-resource-request-schema.json\",\n  \"description\": \"UntagResourceRequest schema from Amazon X-Ray\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-untag-resource-request-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: UntagResourceRequest
---
