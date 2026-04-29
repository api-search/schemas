---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: Error
  type: object
- description: The unique request identifier
  name: RequestId
  type: string
provider_name: Amazon SNS
provider_slug: amazon-sns
schema_file: json-schema/amazon-sns-error-response-schema.json
slug: amazon-sns-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Error\": {\n      \"type\": \"object\"\n    },\n    \"RequestId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique request identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/json-schema/amazon-sns-error-response-schema.json
tags:
- AWS
- Email
- Messaging
- Notifications
- Pub/Sub
- Push Notifications
- SMS
title: ErrorResponse
---
