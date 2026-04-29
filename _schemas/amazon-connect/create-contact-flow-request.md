---
description: CreateContactFlowRequest schema from Amazon Connect Service API
layout: schema
name: CreateContactFlowRequest
properties_list:
- description: The name of the contact flow.
  name: Name
  type: string
- description: The type of the contact flow.
  name: Type
  type: string
- description: The description of the contact flow.
  name: Description
  type: string
- description: The content of the contact flow.
  name: Content
  type: string
- description: ''
  name: Tags
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-contact-flow-request-schema.json
slug: create-contact-flow-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-contact-flow-request-schema.json\",\n  \"title\": \"CreateContactFlowRequest\",\n  \"description\": \"CreateContactFlowRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the contact flow.\",\n      \"example\": \"My Contact Flow\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the contact flow.\",\n      \"enum\": [\n        \"CONTACT_FLOW\",\n        \"CUSTOMER_QUEUE\",\n        \"CUSTOMER_HOLD\",\n        \"CUSTOMER_WHISPER\",\n        \"AGENT_HOLD\",\n        \"AGENT_WHISPER\",\n        \"OUTBOUND_WHISPER\",\n        \"AGENT_TRANSFER\",\n        \"QUEUE_TRANSFER\"\n      ],\n      \"example\": \"CONTACT_FLOW\"\n    },\n  \
  \  \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the contact flow.\"\n    },\n    \"Content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the contact flow.\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"Content\",\n    \"Name\",\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-contact-flow-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateContactFlowRequest
---
