---
description: DeleteImpersonationRoleRequest schema from Amazon WorkMail API
layout: schema
name: DeleteImpersonationRoleRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: ImpersonationRoleId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-impersonation-role-request-schema.json
slug: workmail-delete-impersonation-role-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"ImpersonationRoleId\"\n  ],\n  \"title\": \"DeleteImpersonationRoleRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization from which to delete the impersonation role.\"\n        }\n      ]\n    },\n    \"ImpersonationRoleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleId\"\n        },\n        {\n          \"description\": \"The ID of the impersonation role to delete.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-impersonation-role-request-schema.json\",\n  \"description\": \"DeleteImpersonationRoleRequest\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-impersonation-role-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteImpersonationRoleRequest
---
