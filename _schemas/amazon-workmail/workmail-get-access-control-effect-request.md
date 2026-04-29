---
description: GetAccessControlEffectRequest schema from Amazon WorkMail API
layout: schema
name: GetAccessControlEffectRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: Action
  type: object
- description: ''
  name: UserId
  type: object
- description: ''
  name: ImpersonationRoleId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-access-control-effect-request-schema.json
slug: workmail-get-access-control-effect-request
source_filename: workmail-get-access-control-effect-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"IpAddress\",\n    \"Action\"\n  ],\n  \"title\": \"GetAccessControlEffectRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier for the organization.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The IPv4 address.\"\n        }\n      ]\n    },\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleAction\"\n        },\n        {\n          \"description\": \"The access protocol action. Valid values include <code>ActiveSync</code>, <code>AutoDiscover</code>, <code>EWS</code>, <code>IMAP</code>, <code>SMTP</code>, <code>WindowsOutlook</code>,\
  \ and <code>WebMail</code>.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The user ID.\"\n        }\n      ]\n    },\n    \"ImpersonationRoleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleId\"\n        },\n        {\n          \"description\": \"The impersonation role ID.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-access-control-effect-request-schema.json\",\n  \"description\": \"GetAccessControlEffectRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-access-control-effect-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetAccessControlEffectRequest
---
