---
description: StartMailboxExportJobResponse schema from Amazon WorkMail API
layout: schema
name: StartMailboxExportJobResponse
properties_list:
- description: ''
  name: JobId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-start-mailbox-export-job-response-schema.json
slug: workmail-start-mailbox-export-job-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxExportJobId\"\n        },\n        {\n          \"description\": \"The job ID.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StartMailboxExportJobResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-start-mailbox-export-job-response-schema.json\",\n  \"description\": \"StartMailboxExportJobResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-start-mailbox-export-job-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: StartMailboxExportJobResponse
---
