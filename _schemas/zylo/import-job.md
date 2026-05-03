---
description: An import job represents an asynchronous task for importing user, license, and activity data into Zylo from a CSV file for a specific subscription.
layout: schema
name: Zylo Import Job
properties_list:
- description: The unique identifier of the import job.
  name: id
  type: string
- description: The subscription ID this import job is associated with.
  name: subscriptionId
  type: string
- description: The current status of the import job.
  name: status
  type: string
- description: The name of the uploaded CSV file.
  name: fileName
  type: string
- description: The number of records processed from the CSV file.
  name: recordsProcessed
  type: integer
- description: The number of records that failed to import.
  name: recordsFailed
  type: integer
- description: The date and time the import job was created.
  name: createdAt
  type: string
- description: The date and time the import job completed.
  name: completedAt
  type: string
- description: Error message if the job failed.
  name: error
  type: string
provider_name: Zylo
provider_slug: zylo
schema_file: json-schema/import-job.json
slug: import-job
source_filename: import-job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"import-job.json\",\n  \"title\": \"Zylo Import Job\",\n  \"description\": \"An import job represents an asynchronous task for importing user, license, and activity data into Zylo from a CSV file for a specific subscription.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the import job.\"\n    },\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription ID this import job is associated with.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the import job.\",\n      \"enum\": [\"pending\", \"processing\", \"completed\", \"failed\"]\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the uploaded CSV file.\"\n    },\n    \"recordsProcessed\": {\n      \"type\":\
  \ \"integer\",\n      \"description\": \"The number of records processed from the CSV file.\"\n    },\n    \"recordsFailed\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of records that failed to import.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the import job was created.\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the import job completed.\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the job failed.\"\n    }\n  },\n  \"required\": [\"id\", \"subscriptionId\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/json-schema/import-job.json
tags:
- Budgets
- SaaS Management
- Spend
title: Zylo Import Job
---
