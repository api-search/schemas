---
description: Request body for updating a job.
layout: schema
name: Update Job Request
properties_list:
- description: ''
  name: priority
  type: integer
- description: ''
  name: lifecycleStatus
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/update-job-request-schema.json
slug: update-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/update-job-request-schema.json\",\n  \"title\": \"Update Job Request\",\n  \"description\": \"Request body for updating a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"priority\": {\n      \"type\": \"integer\"\n    },\n    \"lifecycleStatus\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/update-job-request-schema.json
tags:
- AWS
- Compute
- Media
- Rendering
- Visual Effects
title: Update Job Request
---
