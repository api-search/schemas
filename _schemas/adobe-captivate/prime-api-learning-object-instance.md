---
description: An instance of a learning object representing a specific offering with its own timeline and enrollment settings
layout: schema
name: LearningObjectInstance
properties_list:
- description: Unique identifier for the instance
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-learning-object-instance-schema.json
slug: prime-api-learning-object-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-learning-object-instance-schema.json\",\n  \"title\": \"LearningObjectInstance\",\n  \"description\": \"An instance of a learning object representing a specific offering with its own timeline and enrollment settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the instance\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"learningObjectInstance\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"completionDeadline\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Deadline by which the learner must complete the course\"\n        },\n        \"enrollmentDeadline\": {\n     \
  \     \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Deadline for enrolling in this instance\"\n        },\n        \"isDefault\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the default instance\"\n        },\n        \"seatLimit\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of learners who can enroll\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Current state of the instance\",\n          \"enum\": [\n            \"Active\",\n            \"Retired\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-learning-object-instance-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: LearningObjectInstance
---
