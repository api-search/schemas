---
description: ''
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: tagKeys
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-untagresourceinput-schema.json
slug: step-functions-untagresourceinput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UntagResourceInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {},\n    \"tagKeys\": {}\n  },\n  \"required\": [\n    \"resourceArn\",\n    \"tagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-untagresourceinput-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: UntagResourceInput
---
