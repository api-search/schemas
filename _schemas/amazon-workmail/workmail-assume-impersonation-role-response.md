---
description: AssumeImpersonationRoleResponse schema from Amazon WorkMail API
layout: schema
name: AssumeImpersonationRoleResponse
properties_list:
- description: ''
  name: Token
  type: object
- description: ''
  name: ExpiresIn
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-assume-impersonation-role-response-schema.json
slug: workmail-assume-impersonation-role-response
source_filename: workmail-assume-impersonation-role-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Token\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationToken\"\n        },\n        {\n          \"description\": \"The authentication token for the impersonation role.\"\n        }\n      ]\n    },\n    \"ExpiresIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExpiresIn\"\n        },\n        {\n          \"description\": \"The authentication token's validity, in seconds.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssumeImpersonationRoleResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-assume-impersonation-role-response-schema.json\",\n  \"description\": \"AssumeImpersonationRoleResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-assume-impersonation-role-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: AssumeImpersonationRoleResponse
---
