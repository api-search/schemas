---
description: GetMailboxDetailsRequest schema from Amazon WorkMail API
layout: schema
name: GetMailboxDetailsRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: UserId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-mailbox-details-request-schema.json
slug: workmail-get-mailbox-details-request
source_filename: workmail-get-mailbox-details-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"UserId\"\n  ],\n  \"title\": \"GetMailboxDetailsRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier for the organization that contains the user whose mailbox details are being requested.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier for the user whose mailbox details are being requested.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mailbox-details-request-schema.json\",\n  \"description\": \"GetMailboxDetailsRequest\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-mailbox-details-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetMailboxDetailsRequest
---
