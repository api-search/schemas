---
description: UntagResourceRequest schema from Amazon WorkMail API
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-untag-resource-request-schema.json
slug: workmail-untag-resource-request
source_filename: workmail-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceARN\",\n    \"TagKeys\"\n  ],\n  \"title\": \"UntagResourceRequest\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The resource ARN.\"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"The tag keys.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-untag-resource-request-schema.json\",\n  \"description\": \"UntagResourceRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-untag-resource-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: UntagResourceRequest
---
