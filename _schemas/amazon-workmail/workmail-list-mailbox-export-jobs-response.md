---
description: ListMailboxExportJobsResponse schema from Amazon WorkMail API
layout: schema
name: ListMailboxExportJobsResponse
properties_list:
- description: ''
  name: Jobs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-mailbox-export-jobs-response-schema.json
slug: workmail-list-mailbox-export-jobs-response
source_filename: workmail-list-mailbox-export-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Jobs\"\n        },\n        {\n          \"description\": \"The mailbox export job details.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMailboxExportJobsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mailbox-export-jobs-response-schema.json\",\n  \"description\": \"ListMailboxExportJobsResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mailbox-export-jobs-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListMailboxExportJobsResponse
---
