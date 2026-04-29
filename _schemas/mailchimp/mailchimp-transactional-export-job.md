---
description: Information about a data export job.
layout: schema
name: ExportJob
properties_list:
- description: The unique export job ID.
  name: id
  type: string
- description: When the export was created.
  name: created_at
  type: string
- description: The type of data being exported.
  name: type
  type: string
- description: When the export completed.
  name: finished_at
  type: string
- description: The current state of the export.
  name: state
  type: string
- description: The URL to download the export file (when complete).
  name: result_url
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-export-job-schema.json
slug: mailchimp-transactional-export-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExportJob\",\n  \"type\": \"object\",\n  \"description\": \"Information about a data export job.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique export job ID.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the export was created.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of data being exported.\"\n    },\n    \"finished_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the export completed.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the export.\"\n    },\n    \"result_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to download the export file (when complete).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-export-job-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: ExportJob
---
