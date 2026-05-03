---
description: An export job represents an asynchronous task for exporting subscription data from Zylo. The workflow involves creating the export job and then polling for completion, at which point a download URL is provided.
layout: schema
name: Zylo Export Job
properties_list:
- description: The unique identifier of the export job.
  name: id
  type: string
- description: The current status of the export job.
  name: status
  type: string
- description: The URL to download the exported data. Only available when the job status is completed.
  name: downloadUrl
  type: string
- description: The date and time the export job was created.
  name: createdAt
  type: string
- description: The date and time the export job completed.
  name: completedAt
  type: string
- description: Error message if the job failed.
  name: error
  type: string
provider_name: Zylo
provider_slug: zylo
schema_file: json-schema/export-job.json
slug: export-job
source_filename: export-job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"export-job.json\",\n  \"title\": \"Zylo Export Job\",\n  \"description\": \"An export job represents an asynchronous task for exporting subscription data from Zylo. The workflow involves creating the export job and then polling for completion, at which point a download URL is provided.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the export job.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the export job.\",\n      \"enum\": [\"pending\", \"processing\", \"completed\", \"failed\"]\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to download the exported data. Only available when the job status is completed.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the export job was created.\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the export job completed.\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the job failed.\"\n    }\n  },\n  \"required\": [\"id\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/json-schema/export-job.json
tags:
- Budgets
- SaaS Management
- Spend
title: Zylo Export Job
---
