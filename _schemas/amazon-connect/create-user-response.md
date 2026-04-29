---
description: CreateUserResponse schema from Amazon Connect Service API
layout: schema
name: CreateUserResponse
properties_list:
- description: The identifier of the user account.
  name: UserId
  type: string
- description: The Amazon Resource Name (ARN) of the user account.
  name: UserArn
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-user-response-schema.json
slug: create-user-response
source_filename: create-user-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-user-response-schema.json\",\n  \"title\": \"CreateUserResponse\",\n  \"description\": \"CreateUserResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user account.\",\n      \"example\": \"500123\"\n    },\n    \"UserArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the user account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-user-response-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateUserResponse
---
