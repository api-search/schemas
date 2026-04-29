---
description: GetMailboxDetailsResponse schema from Amazon WorkMail API
layout: schema
name: GetMailboxDetailsResponse
properties_list:
- description: ''
  name: MailboxQuota
  type: object
- description: ''
  name: MailboxSize
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-mailbox-details-response-schema.json
slug: workmail-get-mailbox-details-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MailboxQuota\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxQuota\"\n        },\n        {\n          \"description\": \"The maximum allowed mailbox size, in MB, for the specified user.\"\n        }\n      ]\n    },\n    \"MailboxSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxSize\"\n        },\n        {\n          \"description\": \"The current mailbox size, in MB, for the specified user.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetMailboxDetailsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mailbox-details-response-schema.json\",\n  \"description\": \"GetMailboxDetailsResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mailbox-details-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetMailboxDetailsResponse
---
