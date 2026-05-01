---
description: ''
layout: schema
name: SubscriptionMember
properties_list:
- description: The subscription ARN
  name: SubscriptionArn
  type: string
- description: The subscription owner's AWS account ID
  name: Owner
  type: string
- description: The subscription protocol
  name: Protocol
  type: string
- description: The subscription endpoint
  name: Endpoint
  type: string
- description: The topic ARN that this subscription is associated with
  name: TopicArn
  type: string
provider_name: Amazon SNS
provider_slug: amazon-sns
schema_file: json-schema/amazon-sns-subscription-member-schema.json
slug: amazon-sns-subscription-member
source_filename: amazon-sns-subscription-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionMember\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubscriptionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription ARN\"\n    },\n    \"Owner\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription owner's AWS account ID\"\n    },\n    \"Protocol\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription protocol\"\n    },\n    \"Endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription endpoint\"\n    },\n    \"TopicArn\": {\n      \"type\": \"string\",\n      \"description\": \"The topic ARN that this subscription is associated with\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/json-schema/amazon-sns-subscription-member-schema.json
tags:
- Email
- Messaging
- Notifications
- Pub/Sub
- Push Notifications
- SMS
title: SubscriptionMember
---
