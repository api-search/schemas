---
description: ''
layout: schema
name: ResponseMetadata
properties_list:
- description: The unique request identifier
  name: RequestId
  type: string
provider_name: Amazon SNS
provider_slug: amazon-sns
schema_file: json-schema/amazon-sns-response-metadata-schema.json
slug: amazon-sns-response-metadata
source_filename: amazon-sns-response-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseMetadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique request identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/json-schema/amazon-sns-response-metadata-schema.json
tags:
- AWS
- Email
- Messaging
- Notifications
- Pub/Sub
- Push Notifications
- SMS
title: ResponseMetadata
---
