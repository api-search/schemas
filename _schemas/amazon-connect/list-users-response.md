---
description: ListUsersResponse schema from Amazon Connect Service API
layout: schema
name: ListUsersResponse
properties_list:
- description: ''
  name: UserSummaryList
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/list-users-response-schema.json
slug: list-users-response
source_filename: list-users-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-users-response-schema.json\",\n  \"title\": \"ListUsersResponse\",\n  \"description\": \"ListUsersResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserSummaryList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserSummary\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-users-response-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ListUsersResponse
---
