---
description: DescribeMailboxExportJobRequest schema from Amazon WorkMail API
layout: schema
name: DescribeMailboxExportJobRequest
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: OrganizationId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-mailbox-export-job-request-schema.json
slug: workmail-describe-mailbox-export-job-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"JobId\",\n    \"OrganizationId\"\n  ],\n  \"title\": \"DescribeMailboxExportJobRequest\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MailboxExportJobId\"\n        },\n        {\n          \"description\": \"The mailbox export job ID.\"\n        }\n      ]\n    },\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The organization ID.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-mailbox-export-job-request-schema.json\",\n  \"description\": \"DescribeMailboxExportJobRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-mailbox-export-job-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeMailboxExportJobRequest
---
