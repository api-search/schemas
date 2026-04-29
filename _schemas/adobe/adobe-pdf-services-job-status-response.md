---
description: The status and result of an asynchronous PDF operation job.
layout: schema
name: JobStatusResponse
properties_list:
- description: The current status of the job.
  name: status
  type: string
- description: The output asset information, available when status is done.
  name: asset
  type: object
- description: Error information, available when status is failed.
  name: error
  type: object
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-job-status-response-schema.json
slug: adobe-pdf-services-job-status-response
source_filename: adobe-pdf-services-job-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobStatusResponse\",\n  \"type\": \"object\",\n  \"description\": \"The status and result of an asynchronous PDF operation job.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the job.\"\n    },\n    \"asset\": {\n      \"type\": \"object\",\n      \"description\": \"The output asset information, available when status is done.\"\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error information, available when status is failed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-job-status-response-schema.json
tags:
- Analytics
- Creative Cloud
- Digital Asset Management
- Document Services
- E-Commerce
- E-Signatures
- Experience Cloud
- Generative AI
- Marketing
- PDF
- Work Management
title: JobStatusResponse
---
