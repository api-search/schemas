---
description: Contains summary information about a contact flow.
layout: schema
name: ContactFlowSummary
properties_list:
- description: The identifier of the contact flow.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the contact flow.
  name: Arn
  type: string
- description: The name of the contact flow.
  name: Name
  type: string
- description: The type of contact flow.
  name: ContactFlowType
  type: string
- description: The status of the contact flow.
  name: ContactFlowState
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/contact-flow-summary-schema.json
slug: contact-flow-summary
source_filename: contact-flow-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/contact-flow-summary-schema.json\",\n  \"title\": \"ContactFlowSummary\",\n  \"description\": \"Contains summary information about a contact flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the contact flow.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-77777EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the contact flow.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the contact flow.\",\n      \"example\": \"Default inbound flow\"\n    },\n    \"ContactFlowType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of contact flow.\",\n      \"enum\": [\n        \"CONTACT_FLOW\"\
  ,\n        \"CUSTOMER_QUEUE\",\n        \"CUSTOMER_HOLD\",\n        \"CUSTOMER_WHISPER\",\n        \"AGENT_HOLD\",\n        \"AGENT_WHISPER\",\n        \"OUTBOUND_WHISPER\",\n        \"AGENT_TRANSFER\",\n        \"QUEUE_TRANSFER\"\n      ]\n    },\n    \"ContactFlowState\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the contact flow.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"ARCHIVED\"\n      ],\n      \"example\": \"ACTIVE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/contact-flow-summary-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ContactFlowSummary
---
