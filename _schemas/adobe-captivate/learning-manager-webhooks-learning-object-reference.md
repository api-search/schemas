---
description: Reference to a learning object involved in an event
layout: schema
name: LearningObjectReference
properties_list:
- description: Learning object identifier
  name: loId
  type: string
- description: Type of learning object
  name: loType
  type: string
- description: Learning object name
  name: name
  type: string
- description: Learning object instance identifier
  name: instanceId
  type: string
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/learning-manager-webhooks-learning-object-reference-schema.json
slug: learning-manager-webhooks-learning-object-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-learning-object-reference-schema.json\",\n  \"title\": \"LearningObjectReference\",\n  \"description\": \"Reference to a learning object involved in an event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"loId\": {\n      \"type\": \"string\",\n      \"description\": \"Learning object identifier\"\n    },\n    \"loType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of learning object\",\n      \"enum\": [\n        \"course\",\n        \"learningProgram\",\n        \"certification\",\n        \"jobAid\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Learning object name\"\n    },\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"Learning object instance identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-learning-object-reference-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: LearningObjectReference
---
