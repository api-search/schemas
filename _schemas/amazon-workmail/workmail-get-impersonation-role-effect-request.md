---
description: GetImpersonationRoleEffectRequest schema from Amazon WorkMail API
layout: schema
name: GetImpersonationRoleEffectRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: ImpersonationRoleId
  type: object
- description: ''
  name: TargetUser
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-impersonation-role-effect-request-schema.json
slug: workmail-get-impersonation-role-effect-request
source_filename: workmail-get-impersonation-role-effect-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"ImpersonationRoleId\",\n    \"TargetUser\"\n  ],\n  \"title\": \"GetImpersonationRoleEffectRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization where the impersonation role is defined.\"\n        }\n      ]\n    },\n    \"ImpersonationRoleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleId\"\n        },\n        {\n          \"description\": \"The impersonation role ID to test.\"\n        }\n      ]\n    },\n    \"TargetUser\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityIdentifier\"\n        },\n        {\n          \"description\": \"<p>The WorkMail organization user chosen to test the impersonation role. The following identity formats\
  \ are available:</p> <ul> <li> <p>User ID: <code>12345678-1234-1234-1234-123456789012</code> or <code>S-1-1-12-1234567890-123456789-123456789-1234</code> </p> </li> <li> <p>Email address: <code>user@domain.tld</code> </p> </li> <li> <p>User name: <code>user</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-impersonation-role-effect-request-schema.json\",\n  \"description\": \"GetImpersonationRoleEffectRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-impersonation-role-effect-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetImpersonationRoleEffectRequest
---
