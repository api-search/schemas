---
description: ''
layout: schema
name: Tag
properties_list:
- description: The tag key
  name: Key
  type: string
- description: The tag value
  name: Value
  type: string
provider_name: Amazon SNS
provider_slug: amazon-sns
schema_file: json-schema/amazon-sns-tag-schema.json
slug: amazon-sns-tag
source_filename: amazon-sns-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"The tag key\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The tag value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/json-schema/amazon-sns-tag-schema.json
tags:
- AWS
- Email
- Messaging
- Notifications
- Pub/Sub
- Push Notifications
- SMS
title: Tag
---
