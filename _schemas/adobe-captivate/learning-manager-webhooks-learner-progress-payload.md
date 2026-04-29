---
description: LearnerProgressPayload schema from Adobe Learning Manager Webhooks
layout: schema
name: LearnerProgressPayload
properties_list: []
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/learning-manager-webhooks-learner-progress-payload-schema.json
slug: learning-manager-webhooks-learner-progress-payload
source_filename: learning-manager-webhooks-learner-progress-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-learner-progress-payload-schema.json\",\n  \"title\": \"LearnerProgressPayload\",\n  \"description\": \"LearnerProgressPayload schema from Adobe Learning Manager Webhooks\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"description\": \"Base schema for all webhook event payloads\",\n      \"required\": [\n        \"eventType\",\n        \"eventId\",\n        \"accountId\",\n        \"timestamp\"\n      ],\n      \"properties\": {\n        \"eventType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of event that triggered this webhook\"\n        },\n        \"eventId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for this event instance\"\n        },\n        \"accountId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The Learning Manager account ID\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the event occurred\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The system component that generated the event\",\n          \"enum\": [\n            \"learner\",\n            \"admin\",\n            \"manager\",\n            \"system\",\n            \"api\"\n          ]\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"eventType\": {\n          \"const\": \"LEARNER_PROGRESS\"\n        },\n        \"learner\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to a learner involved in an event\",\n          \"properties\": {\n            \"userId\": {\n              \"type\": \"string\",\n           \
  \   \"description\": \"Unique user identifier\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Learner's full name\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"format\": \"email\",\n              \"description\": \"Learner's email address\"\n            }\n          }\n        },\n        \"learningObject\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to a learning object involved in an event\",\n          \"properties\": {\n            \"loId\": {\n              \"type\": \"string\",\n              \"description\": \"Learning object identifier\"\n            },\n            \"loType\": {\n              \"type\": \"string\",\n              \"description\": \"Type of learning object\",\n              \"enum\": [\n                \"course\",\n                \"learningProgram\",\n                \"certification\",\n                \"jobAid\"\
  \n              ]\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Learning object name\"\n            },\n            \"instanceId\": {\n              \"type\": \"string\",\n              \"description\": \"Learning object instance identifier\"\n            }\n          }\n        },\n        \"enrollmentId\": {\n          \"type\": \"string\",\n          \"description\": \"Enrollment identifier\"\n        },\n        \"progressPercent\": {\n          \"type\": \"integer\",\n          \"description\": \"Current progress percentage\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-learner-progress-payload-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: LearnerProgressPayload
---
