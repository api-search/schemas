---
description: Contains summary information about a user.
layout: schema
name: UserSummary
properties_list:
- description: The identifier of the user account.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the user account.
  name: Arn
  type: string
- description: The Amazon Connect user name of the user account.
  name: Username
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/user-summary-schema.json
slug: user-summary
source_filename: user-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/user-summary-schema.json\",\n  \"title\": \"UserSummary\",\n  \"description\": \"Contains summary information about a user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user account.\",\n      \"example\": \"500123\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the user account.\",\n      \"example\": \"arn:aws:connect:us-east-1:123456789012:instance/a1b2c3d4/agent/500123\"\n    },\n    \"Username\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Connect user name of the user account.\",\n      \"example\": \"jsmith\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/user-summary-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: UserSummary
---
