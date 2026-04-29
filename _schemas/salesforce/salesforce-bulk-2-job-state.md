---
description: The current state of a Bulk API 2.0 job, indicating where it is in its lifecycle.
layout: schema
name: JobState
properties_list: []
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-bulk-2-job-state-schema.json
slug: salesforce-bulk-2-job-state
source_json: "{\n  \"type\": \"string\",\n  \"description\": \"The current state of a Bulk API 2.0 job, indicating where it is in its lifecycle.\\n\",\n  \"enum\": [\n    \"Open\",\n    \"UploadComplete\",\n    \"InProgress\",\n    \"JobComplete\",\n    \"Failed\",\n    \"Aborted\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobState\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-bulk-2-job-state-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: JobState
---
