---
description: CreateImpersonationRoleResponse schema from Amazon WorkMail API
layout: schema
name: CreateImpersonationRoleResponse
properties_list:
- description: ''
  name: ImpersonationRoleId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-create-impersonation-role-response-schema.json
slug: workmail-create-impersonation-role-response
source_filename: workmail-create-impersonation-role-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImpersonationRoleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleId\"\n        },\n        {\n          \"description\": \"The new impersonation role ID.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateImpersonationRoleResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-impersonation-role-response-schema.json\",\n  \"description\": \"CreateImpersonationRoleResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-impersonation-role-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: CreateImpersonationRoleResponse
---
