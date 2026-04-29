---
description: UpdateMailboxQuotaRequest schema from Amazon WorkMail API
layout: schema
name: UpdateMailboxQuotaRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: UserId
  type: object
- description: ''
  name: MailboxQuota
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-update-mailbox-quota-request-schema.json
slug: workmail-update-mailbox-quota-request
source_filename: workmail-update-mailbox-quota-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"UserId\",\n    \"MailboxQuota\"\n  ],\n  \"title\": \"UpdateMailboxQuotaRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier for the organization that contains the user for whom to update the mailbox quota.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifer for the user for whom to update the mailbox quota.\"\n        }\n      ]\n    },\n    \"MailboxQuota\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxQuota\"\n        },\n        {\n          \"description\": \"The updated mailbox quota, in MB, for the specified user.\"\n        }\n   \
  \   ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-mailbox-quota-request-schema.json\",\n  \"description\": \"UpdateMailboxQuotaRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-mailbox-quota-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: UpdateMailboxQuotaRequest
---
