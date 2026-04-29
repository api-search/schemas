---
description: SkillAchievedPayload schema from Adobe Learning Manager Webhooks
layout: schema
name: SkillAchievedPayload
properties_list: []
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/learning-manager-webhooks-skill-achieved-payload-schema.json
slug: learning-manager-webhooks-skill-achieved-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-skill-achieved-payload-schema.json\",\n  \"title\": \"SkillAchievedPayload\",\n  \"description\": \"SkillAchievedPayload schema from Adobe Learning Manager Webhooks\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"description\": \"Base schema for all webhook event payloads\",\n      \"required\": [\n        \"eventType\",\n        \"eventId\",\n        \"accountId\",\n        \"timestamp\"\n      ],\n      \"properties\": {\n        \"eventType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of event that triggered this webhook\"\n        },\n        \"eventId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for this event instance\"\n        },\n        \"accountId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The Learning Manager account ID\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the event occurred\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The system component that generated the event\",\n          \"enum\": [\n            \"learner\",\n            \"admin\",\n            \"manager\",\n            \"system\",\n            \"api\"\n          ]\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"eventType\": {\n          \"const\": \"SKILL_ACHIEVED\"\n        },\n        \"learner\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to a learner involved in an event\",\n          \"properties\": {\n            \"userId\": {\n              \"type\": \"string\",\n             \
  \ \"description\": \"Unique user identifier\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Learner's full name\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"format\": \"email\",\n              \"description\": \"Learner's email address\"\n            }\n          }\n        },\n        \"skill\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"skillId\": {\n              \"type\": \"string\",\n              \"description\": \"Skill identifier\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Skill name\"\n            },\n            \"levelName\": {\n              \"type\": \"string\",\n              \"description\": \"Skill level name achieved\"\n            },\n            \"credits\": {\n              \"type\": \"number\",\n              \"description\": \"Skill credits earned\"\
  \n            }\n          }\n        },\n        \"dateAchieved\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Achievement timestamp\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-skill-achieved-payload-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: SkillAchievedPayload
---
