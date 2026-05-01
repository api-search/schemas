---
description: UntagResourceInput schema from Amazon Proton API
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: tagKeys
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-untag-resource-input-schema.json
slug: amazon-proton-untag-resource-input
source_filename: amazon-proton-untag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-untag-resource-input-schema.json\",\n  \"title\": \"UntagResourceInput\",\n  \"description\": \"UntagResourceInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource to remove customer tags from.\"\n        }\n      ]\n    },\n    \"tagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"A list of customer tag keys that indicate the customer tags to be removed from the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\",\n    \"tagKeys\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-untag-resource-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UntagResourceInput
---
