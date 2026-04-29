---
description: Response returned immediately after an async generation job is submitted
layout: schema
name: AsyncJobSubmitted
properties_list:
- description: Unique identifier for the generation job
  name: jobId
  type: string
- description: URL to poll for job status updates
  name: statusUrl
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-async-job-submitted-schema.json
slug: adobe-creative-suite-firefly-async-job-submitted
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-async-job-submitted-schema.json\",\n  \"title\": \"AsyncJobSubmitted\",\n  \"description\": \"Response returned immediately after an async generation job is submitted\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the generation job\",\n      \"example\": \"urn:firefly:jobs:abc123def456\"\n    },\n    \"statusUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to poll for job status updates\",\n      \"example\": \"https://firefly-api.adobe.io/v3/status/urn:firefly:jobs:abc123def456\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-async-job-submitted-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: AsyncJobSubmitted
---
