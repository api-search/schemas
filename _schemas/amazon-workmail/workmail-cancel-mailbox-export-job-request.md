---
description: CancelMailboxExportJobRequest schema from Amazon WorkMail API
layout: schema
name: CancelMailboxExportJobRequest
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: JobId
  type: object
- description: ''
  name: OrganizationId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-cancel-mailbox-export-job-request-schema.json
slug: workmail-cancel-mailbox-export-job-request
source_filename: workmail-cancel-mailbox-export-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ClientToken\",\n    \"JobId\",\n    \"OrganizationId\"\n  ],\n  \"title\": \"CancelMailboxExportJobRequest\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token for the client request.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxExportJobId\"\n        },\n        {\n          \"description\": \"The job ID.\"\n        }\n      ]\n    },\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The organization ID.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-cancel-mailbox-export-job-request-schema.json\"\
  ,\n  \"description\": \"CancelMailboxExportJobRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-cancel-mailbox-export-job-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: CancelMailboxExportJobRequest
---
