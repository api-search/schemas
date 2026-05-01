---
description: PutMailboxPermissionsRequest schema from Amazon WorkMail API
layout: schema
name: PutMailboxPermissionsRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: EntityId
  type: object
- description: ''
  name: GranteeId
  type: object
- description: ''
  name: PermissionValues
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-put-mailbox-permissions-request-schema.json
slug: workmail-put-mailbox-permissions-request
source_filename: workmail-put-mailbox-permissions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"EntityId\",\n    \"GranteeId\",\n    \"PermissionValues\"\n  ],\n  \"title\": \"PutMailboxPermissionsRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier of the organization under which the user, group, or resource exists.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the user, group, or resource for which to update mailbox permissions.\"\n        }\n      ]\n    },\n    \"GranteeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the user, group,\
  \ or resource to which to grant the permissions.\"\n        }\n      ]\n    },\n    \"PermissionValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionValues\"\n        },\n        {\n          \"description\": \"The permissions granted to the grantee. SEND_AS allows the grantee to send email as the owner of the mailbox (the grantee is not mentioned on these emails). SEND_ON_BEHALF allows the grantee to send email on behalf of the owner of the mailbox (the grantee is not mentioned as the physical sender of these emails). FULL_ACCESS allows the grantee full access to the mailbox, irrespective of other folder-level permissions set on the mailbox.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-mailbox-permissions-request-schema.json\",\n  \"description\": \"PutMailboxPermissionsRequest\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-mailbox-permissions-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: PutMailboxPermissionsRequest
---
