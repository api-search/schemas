---
description: Reference to a learner involved in an event
layout: schema
name: LearnerReference
properties_list:
- description: Unique user identifier
  name: userId
  type: string
- description: Learner's full name
  name: name
  type: string
- description: Learner's email address
  name: email
  type: string
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/learning-manager-webhooks-learner-reference-schema.json
slug: learning-manager-webhooks-learner-reference
source_filename: learning-manager-webhooks-learner-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-learner-reference-schema.json\",\n  \"title\": \"LearnerReference\",\n  \"description\": \"Reference to a learner involved in an event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Learner's full name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Learner's email address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/learning-manager-webhooks-learner-reference-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: LearnerReference
---
