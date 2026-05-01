---
description: Contains information about a contact flow.
layout: schema
name: ContactFlow
properties_list:
- description: The Amazon Resource Name (ARN) of the contact flow.
  name: Arn
  type: string
- description: The identifier of the contact flow.
  name: Id
  type: string
- description: The name of the contact flow.
  name: Name
  type: string
- description: The type of the contact flow.
  name: Type
  type: string
- description: The state of the contact flow.
  name: State
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
schema_file: json-schema/contact-flow-schema.json
slug: contact-flow
source_filename: contact-flow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/contact-flow-schema.json\",\n  \"title\": \"ContactFlow\",\n  \"description\": \"Contains information about a contact flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the contact flow.\"\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the contact flow.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-77777EXAMPLE\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the contact flow.\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the contact flow.\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the contact flow.\"\
  ,\n      \"enum\": [\n        \"ACTIVE\",\n        \"ARCHIVED\"\n      ]\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the contact flow.\"\n    },\n    \"Content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the contact flow.\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/contact-flow-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ContactFlow
---
