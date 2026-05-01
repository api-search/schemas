---
description: CreateUserResponse schema from Amazon WorkMail API
layout: schema
name: CreateUserResponse
properties_list:
- description: ''
  name: UserId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-create-user-response-schema.json
slug: workmail-create-user-response
source_filename: workmail-create-user-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier for the new user.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateUserResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-user-response-schema.json\",\n  \"description\": \"CreateUserResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-user-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: CreateUserResponse
---
