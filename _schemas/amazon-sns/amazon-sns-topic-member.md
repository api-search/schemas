---
description: ''
layout: schema
name: TopicMember
properties_list:
- description: The ARN of the topic
  name: TopicArn
  type: string
provider_name: Amazon SNS
provider_slug: amazon-sns
schema_file: json-schema/amazon-sns-topic-member-schema.json
slug: amazon-sns-topic-member
source_filename: amazon-sns-topic-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TopicMember\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TopicArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the topic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/json-schema/amazon-sns-topic-member-schema.json
tags:
- Email
- Messaging
- Notifications
- Pub/Sub
- Push Notifications
- SMS
title: TopicMember
---
