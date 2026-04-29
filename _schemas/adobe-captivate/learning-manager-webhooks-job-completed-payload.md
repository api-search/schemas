---
description: JobCompletedPayload schema from Adobe Learning Manager Webhooks
layout: schema
name: JobCompletedPayload
properties_list: []
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/learning-manager-webhooks-job-completed-payload-schema.json
slug: learning-manager-webhooks-job-completed-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-job-completed-payload-schema.json\",\n  \"title\": \"JobCompletedPayload\",\n  \"description\": \"JobCompletedPayload schema from Adobe Learning Manager Webhooks\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"description\": \"Base schema for all webhook event payloads\",\n      \"required\": [\n        \"eventType\",\n        \"eventId\",\n        \"accountId\",\n        \"timestamp\"\n      ],\n      \"properties\": {\n        \"eventType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of event that triggered this webhook\"\n        },\n        \"eventId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for this event instance\"\n        },\n        \"accountId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The Learning Manager account ID\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the event occurred\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The system component that generated the event\",\n          \"enum\": [\n            \"learner\",\n            \"admin\",\n            \"manager\",\n            \"system\",\n            \"api\"\n          ]\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"eventType\": {\n          \"const\": \"JOB_COMPLETED\"\n        },\n        \"job\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"jobId\": {\n              \"type\": \"string\",\n              \"description\": \"Job identifier\"\n            },\n            \"jobType\": {\n \
  \             \"type\": \"string\",\n              \"description\": \"Type of bulk operation\",\n              \"enum\": [\n                \"userImport\",\n                \"learnerTranscriptExport\",\n                \"trainingReportExport\"\n              ]\n            },\n            \"status\": {\n              \"type\": \"string\",\n              \"description\": \"Final job status\",\n              \"enum\": [\n                \"Completed\",\n                \"Failed\"\n              ]\n            },\n            \"downloadUrl\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL to download results (for export jobs)\"\n            },\n            \"recordsProcessed\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of records processed\"\n            },\n            \"recordsFailed\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of records that failed\"\
  \n            }\n          }\n        },\n        \"dateCompleted\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Job completion timestamp\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-job-completed-payload-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: JobCompletedPayload
---
