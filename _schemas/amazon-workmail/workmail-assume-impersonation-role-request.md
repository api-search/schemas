---
description: AssumeImpersonationRoleRequest schema from Amazon WorkMail API
layout: schema
name: AssumeImpersonationRoleRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: ImpersonationRoleId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-assume-impersonation-role-request-schema.json
slug: workmail-assume-impersonation-role-request
source_filename: workmail-assume-impersonation-role-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"ImpersonationRoleId\"\n  ],\n  \"title\": \"AssumeImpersonationRoleRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization under which the impersonation role will be assumed.\"\n        }\n      ]\n    },\n    \"ImpersonationRoleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleId\"\n        },\n        {\n          \"description\": \"The impersonation role ID to assume.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-assume-impersonation-role-request-schema.json\",\n  \"description\": \"AssumeImpersonationRoleRequest\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-assume-impersonation-role-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: AssumeImpersonationRoleRequest
---
