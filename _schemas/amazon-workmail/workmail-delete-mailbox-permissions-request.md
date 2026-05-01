---
description: DeleteMailboxPermissionsRequest schema from Amazon WorkMail API
layout: schema
name: DeleteMailboxPermissionsRequest
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
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-mailbox-permissions-request-schema.json
slug: workmail-delete-mailbox-permissions-request
source_filename: workmail-delete-mailbox-permissions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"EntityId\",\n    \"GranteeId\"\n  ],\n  \"title\": \"DeleteMailboxPermissionsRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier of the organization under which the member (user or group) exists.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the member (user or group) that owns the mailbox.\"\n        }\n      ]\n    },\n    \"GranteeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier of the member (user or group) for which to delete granted permissions.\"\
  \n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-mailbox-permissions-request-schema.json\",\n  \"description\": \"DeleteMailboxPermissionsRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-mailbox-permissions-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteMailboxPermissionsRequest
---
