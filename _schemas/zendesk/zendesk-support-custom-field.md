---
description: A custom field key-value pair.
layout: schema
name: CustomField
properties_list:
- description: The ID of the custom field.
  name: id
  type: integer
- description: The value of the custom field.
  name: value
  type: string
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-custom-field-schema.json
slug: zendesk-support-custom-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomField\",\n  \"type\": \"object\",\n  \"description\": \"A custom field key-value pair.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the custom field.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the custom field.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-custom-field-schema.json
tags:
- Chat
- CRM
- Help Center
- Sell
- Support
- T1
- Talk
- Ticketing
- Tickets
title: CustomField
---
