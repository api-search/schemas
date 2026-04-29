---
description: CourseUpdatedPayload schema from Adobe Learning Manager Webhooks
layout: schema
name: CourseUpdatedPayload
properties_list: []
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/learning-manager-webhooks-course-updated-payload-schema.json
slug: learning-manager-webhooks-course-updated-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-course-updated-payload-schema.json\",\n  \"title\": \"CourseUpdatedPayload\",\n  \"description\": \"CourseUpdatedPayload schema from Adobe Learning Manager Webhooks\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"description\": \"Base schema for all webhook event payloads\",\n      \"required\": [\n        \"eventType\",\n        \"eventId\",\n        \"accountId\",\n        \"timestamp\"\n      ],\n      \"properties\": {\n        \"eventType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of event that triggered this webhook\"\n        },\n        \"eventId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for this event instance\"\n        },\n        \"accountId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The Learning Manager account ID\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the event occurred\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The system component that generated the event\",\n          \"enum\": [\n            \"learner\",\n            \"admin\",\n            \"manager\",\n            \"system\",\n            \"api\"\n          ]\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"eventType\": {\n          \"const\": \"COURSE_UPDATED\"\n        },\n        \"learningObject\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to a learning object involved in an event\",\n          \"properties\": {\n            \"loId\": {\n              \"type\": \"string\",\n\
  \              \"description\": \"Learning object identifier\"\n            },\n            \"loType\": {\n              \"type\": \"string\",\n              \"description\": \"Type of learning object\",\n              \"enum\": [\n                \"course\",\n                \"learningProgram\",\n                \"certification\",\n                \"jobAid\"\n              ]\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Learning object name\"\n            },\n            \"instanceId\": {\n              \"type\": \"string\",\n              \"description\": \"Learning object instance identifier\"\n            }\n          }\n        },\n        \"updatedBy\": {\n          \"type\": \"string\",\n          \"description\": \"User ID of who made the update\"\n        },\n        \"updatedFields\": {\n          \"type\": \"array\",\n          \"description\": \"List of fields that were modified\",\n          \"items\": {\n \
  \           \"type\": \"string\"\n          }\n        },\n        \"dateUpdated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Update timestamp\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-course-updated-payload-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: CourseUpdatedPayload
---
