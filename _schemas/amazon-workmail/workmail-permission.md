---
description: Permission granted to a user, group, or resource to access a certain aspect of another user, group, or resource mailbox.
layout: schema
name: Permission
properties_list:
- description: ''
  name: GranteeId
  type: object
- description: ''
  name: GranteeType
  type: object
- description: ''
  name: PermissionValues
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-permission-schema.json
slug: workmail-permission
source_filename: workmail-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"GranteeId\",\n    \"GranteeType\",\n    \"PermissionValues\"\n  ],\n  \"properties\": {\n    \"GranteeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the user, group, or resource to which the permissions are granted.\"\n        }\n      ]\n    },\n    \"GranteeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberType\"\n        },\n        {\n          \"description\": \"The type of user, group, or resource referred to in GranteeId.\"\n        }\n      ]\n    },\n    \"PermissionValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionValues\"\n        },\n        {\n          \"description\": \"The permissions granted to the grantee. SEND_AS allows the grantee to send email as the owner of the mailbox (the grantee is not\
  \ mentioned on these emails). SEND_ON_BEHALF allows the grantee to send email on behalf of the owner of the mailbox (the grantee is not mentioned as the physical sender of these emails). FULL_ACCESS allows the grantee full access to the mailbox, irrespective of other folder-level permissions set on the mailbox.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Permission granted to a user, group, or resource to access a certain aspect of another user, group, or resource mailbox.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Permission\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-permission-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-permission-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: Permission
---
