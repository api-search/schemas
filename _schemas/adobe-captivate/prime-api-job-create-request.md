---
description: Request body for creating a bulk job
layout: schema
name: JobCreateRequest
properties_list:
- description: ''
  name: data
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-job-create-request-schema.json
slug: prime-api-job-create-request
source_filename: prime-api-job-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-job-create-request-schema.json\",\n  \"title\": \"JobCreateRequest\",\n  \"description\": \"Request body for creating a bulk job\",\n  \"type\": \"object\",\n  \"required\": [\n    \"data\"\n  ],\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"type\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"job\"\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"required\": [\n            \"jobType\"\n          ],\n          \"properties\": {\n            \"jobType\": {\n              \"type\": \"string\",\n              \"description\": \"The type of bulk operation\",\n              \"enum\": [\n                \"userImport\"\
  ,\n                \"learnerTranscriptExport\",\n                \"trainingReportExport\"\n              ]\n            },\n            \"description\": {\n              \"type\": \"string\",\n              \"description\": \"Description for this job\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-job-create-request-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: JobCreateRequest
---
