---
description: ResetPasswordRequest schema from Amazon WorkMail API
layout: schema
name: ResetPasswordRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: UserId
  type: object
- description: ''
  name: Password
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-reset-password-request-schema.json
slug: workmail-reset-password-request
source_filename: workmail-reset-password-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"UserId\",\n    \"Password\"\n  ],\n  \"title\": \"ResetPasswordRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier of the organization that contains the user for which the password is reset.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the user for whom the password is reset.\"\n        }\n      ]\n    },\n    \"Password\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Password\"\n        },\n        {\n          \"description\": \"The new password for the user.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-reset-password-request-schema.json\",\n  \"description\": \"ResetPasswordRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-reset-password-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ResetPasswordRequest
---
