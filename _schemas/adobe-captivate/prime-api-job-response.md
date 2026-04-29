---
description: Single job response
layout: schema
name: JobResponse
properties_list:
- description: A bulk import/export job
  name: data
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-job-response-schema.json
slug: prime-api-job-response
source_filename: prime-api-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-job-response-schema.json\",\n  \"title\": \"JobResponse\",\n  \"description\": \"Single job response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"A bulk import/export job\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique job identifier\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"job\"\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"dateCreated\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"description\": \"Timestamp when the job was created\"\n            },\n            \"dateCompleted\"\
  : {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"description\": \"Timestamp when the job completed\"\n            },\n            \"description\": {\n              \"type\": \"string\",\n              \"description\": \"Job description\"\n            },\n            \"downloadUrl\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL to download the job result file (for export jobs)\"\n            },\n            \"jobType\": {\n              \"type\": \"string\",\n              \"description\": \"The type of bulk operation\",\n              \"enum\": [\n                \"userImport\",\n                \"learnerTranscriptExport\",\n                \"trainingReportExport\"\n              ]\n            },\n            \"status\": {\n              \"type\": \"string\",\n              \"description\": \"Current job status\",\n              \"enum\": [\n                \"Submitted\"\
  ,\n                \"InProgress\",\n                \"Completed\",\n                \"Failed\"\n              ]\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-job-response-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: JobResponse
---
