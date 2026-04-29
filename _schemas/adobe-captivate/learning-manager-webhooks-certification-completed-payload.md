---
description: CertificationCompletedPayload schema from Adobe Learning Manager Webhooks
layout: schema
name: CertificationCompletedPayload
properties_list: []
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/learning-manager-webhooks-certification-completed-payload-schema.json
slug: learning-manager-webhooks-certification-completed-payload
source_filename: learning-manager-webhooks-certification-completed-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-certification-completed-payload-schema.json\",\n  \"title\": \"CertificationCompletedPayload\",\n  \"description\": \"CertificationCompletedPayload schema from Adobe Learning Manager Webhooks\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"description\": \"Base schema for all webhook event payloads\",\n      \"required\": [\n        \"eventType\",\n        \"eventId\",\n        \"accountId\",\n        \"timestamp\"\n      ],\n      \"properties\": {\n        \"eventType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of event that triggered this webhook\"\n        },\n        \"eventId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for this event instance\"\n  \
  \      },\n        \"accountId\": {\n          \"type\": \"string\",\n          \"description\": \"The Learning Manager account ID\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the event occurred\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The system component that generated the event\",\n          \"enum\": [\n            \"learner\",\n            \"admin\",\n            \"manager\",\n            \"system\",\n            \"api\"\n          ]\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"eventType\": {\n          \"const\": \"CERTIFICATION_COMPLETED\"\n        },\n        \"learner\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to a learner involved in an event\",\n          \"properties\": {\n            \"userId\": {\n         \
  \     \"type\": \"string\",\n              \"description\": \"Unique user identifier\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Learner's full name\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"format\": \"email\",\n              \"description\": \"Learner's email address\"\n            }\n          }\n        },\n        \"certification\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"certificationId\": {\n              \"type\": \"string\",\n              \"description\": \"Certification identifier\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Certification name\"\n            },\n            \"instanceId\": {\n              \"type\": \"string\",\n              \"description\": \"Certification instance identifier\"\n            }\n          }\n        },\n       \
  \ \"completedOn\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Completion timestamp\"\n        },\n        \"validUntil\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Certification validity expiration date\"\n        },\n        \"recertificationDeadline\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Deadline for recertification\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-certification-completed-payload-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: CertificationCompletedPayload
---
