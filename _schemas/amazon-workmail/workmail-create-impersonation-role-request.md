---
description: CreateImpersonationRoleRequest schema from Amazon WorkMail API
layout: schema
name: CreateImpersonationRoleRequest
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: OrganizationId
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
schema_file: json-schema/workmail-create-impersonation-role-request-schema.json
slug: workmail-create-impersonation-role-request
source_filename: workmail-create-impersonation-role-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"Name\",\n    \"Type\",\n    \"Rules\"\n  ],\n  \"title\": \"CreateImpersonationRoleRequest\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token for the client request.\"\n        }\n      ]\n    },\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization to create the new impersonation role within.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleName\"\n        },\n        {\n          \"description\": \"The name of the new impersonation role.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleType\"\n        },\n        {\n          \"description\": \"The impersonation role's type. The available impersonation role types are <code>READ_ONLY</code> or <code>FULL_ACCESS</code>.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleDescription\"\n        },\n        {\n          \"description\": \"The description of the new impersonation role.\"\n        }\n      ]\n    },\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRuleList\"\n        },\n        {\n          \"description\": \"The list of rules for the impersonation role.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-impersonation-role-request-schema.json\"\
  ,\n  \"description\": \"CreateImpersonationRoleRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-impersonation-role-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: CreateImpersonationRoleRequest
---
