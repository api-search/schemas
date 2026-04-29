---
description: UpdateImpersonationRoleRequest schema from Amazon WorkMail API
layout: schema
name: UpdateImpersonationRoleRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: ImpersonationRoleId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Rules
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-update-impersonation-role-request-schema.json
slug: workmail-update-impersonation-role-request
source_filename: workmail-update-impersonation-role-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"ImpersonationRoleId\",\n    \"Name\",\n    \"Type\",\n    \"Rules\"\n  ],\n  \"title\": \"UpdateImpersonationRoleRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization that contains the impersonation role to update.\"\n        }\n      ]\n    },\n    \"ImpersonationRoleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleId\"\n        },\n        {\n          \"description\": \"The ID of the impersonation role to update.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleName\"\n        },\n        {\n          \"description\": \"The updated impersonation role name.\"\n        }\n      ]\n   \
  \ },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleType\"\n        },\n        {\n          \"description\": \"The updated impersonation role type.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleDescription\"\n        },\n        {\n          \"description\": \"The updated impersonation role description.\"\n        }\n      ]\n    },\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRuleList\"\n        },\n        {\n          \"description\": \"The updated list of rules.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-impersonation-role-request-schema.json\",\n  \"description\": \"UpdateImpersonationRoleRequest\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-impersonation-role-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: UpdateImpersonationRoleRequest
---
