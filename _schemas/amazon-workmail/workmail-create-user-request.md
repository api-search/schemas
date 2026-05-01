---
description: CreateUserRequest schema from Amazon WorkMail API
layout: schema
name: CreateUserRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: DisplayName
  type: object
- description: ''
  name: Password
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-create-user-request-schema.json
slug: workmail-create-user-request
source_filename: workmail-create-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"Name\",\n    \"DisplayName\",\n    \"Password\"\n  ],\n  \"title\": \"CreateUserRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier of the organization for which the user is created.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"The name for the new user. WorkMail directory user names have a maximum length of 64. All others have a maximum length of 20.\"\n        }\n      ]\n    },\n    \"DisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The display name for the new user.\"\n        }\n      ]\n\
  \    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Password\"\n        },\n        {\n          \"description\": \"The password for the new user.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-user-request-schema.json\",\n  \"description\": \"CreateUserRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-user-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: CreateUserRequest
---
