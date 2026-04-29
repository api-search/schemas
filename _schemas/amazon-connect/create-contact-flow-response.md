---
description: CreateContactFlowResponse schema from Amazon Connect Service API
layout: schema
name: CreateContactFlowResponse
properties_list:
- description: The identifier of the contact flow.
  name: ContactFlowId
  type: string
- description: The Amazon Resource Name (ARN) of the contact flow.
  name: ContactFlowArn
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-contact-flow-response-schema.json
slug: create-contact-flow-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-contact-flow-response-schema.json\",\n  \"title\": \"CreateContactFlowResponse\",\n  \"description\": \"CreateContactFlowResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContactFlowId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the contact flow.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-77777EXAMPLE\"\n    },\n    \"ContactFlowArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the contact flow.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-contact-flow-response-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateContactFlowResponse
---
