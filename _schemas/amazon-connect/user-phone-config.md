---
description: Contains information about the phone configuration settings for a user.
layout: schema
name: UserPhoneConfig
properties_list:
- description: The phone type.
  name: PhoneType
  type: string
- description: The Auto accept setting.
  name: AutoAccept
  type: boolean
- description: The After Contact Work (ACW) timeout setting, in seconds.
  name: AfterContactWorkTimeLimit
  type: integer
- description: The phone number for the user's desk phone.
  name: DeskPhoneNumber
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/user-phone-config-schema.json
slug: user-phone-config
source_filename: user-phone-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/user-phone-config-schema.json\",\n  \"title\": \"UserPhoneConfig\",\n  \"description\": \"Contains information about the phone configuration settings for a user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PhoneType\": {\n      \"type\": \"string\",\n      \"description\": \"The phone type.\",\n      \"enum\": [\n        \"SOFT_PHONE\",\n        \"DESK_PHONE\"\n      ],\n      \"example\": \"SOFT_PHONE\"\n    },\n    \"AutoAccept\": {\n      \"type\": \"boolean\",\n      \"description\": \"The Auto accept setting.\",\n      \"example\": false\n    },\n    \"AfterContactWorkTimeLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"The After Contact Work (ACW) timeout setting, in seconds.\",\n      \"example\": 0\n    },\n    \"DeskPhoneNumber\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"The phone number for the user's desk phone.\"\n    }\n  },\n  \"required\": [\n    \"PhoneType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/user-phone-config-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: UserPhoneConfig
---
