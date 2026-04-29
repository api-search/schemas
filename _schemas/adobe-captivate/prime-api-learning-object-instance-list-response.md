---
description: Paginated list of learning object instances
layout: schema
name: LearningObjectInstanceListResponse
properties_list:
- description: ''
  name: data
  type: array
- description: Pagination links following JSON:API conventions
  name: links
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-learning-object-instance-list-response-schema.json
slug: prime-api-learning-object-instance-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-learning-object-instance-list-response-schema.json\",\n  \"title\": \"LearningObjectInstanceListResponse\",\n  \"description\": \"Paginated list of learning object instances\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"An instance of a learning object representing a specific offering with its own timeline and enrollment settings\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the instance\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"const\": \"learningObjectInstance\"\n          },\n          \"attributes\": {\n            \"type\":\
  \ \"object\",\n            \"properties\": {\n              \"completionDeadline\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Deadline by which the learner must complete the course\"\n              },\n              \"enrollmentDeadline\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Deadline for enrolling in this instance\"\n              },\n              \"isDefault\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether this is the default instance\"\n              },\n              \"seatLimit\": {\n                \"type\": \"integer\",\n                \"description\": \"Maximum number of learners who can enroll\"\n              },\n              \"state\": {\n                \"type\": \"string\",\n                \"description\": \"Current state of the instance\",\n                \"enum\": [\n\
  \                  \"Active\",\n                  \"Retired\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination links following JSON:API conventions\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the current page\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the next page\"\n        },\n        \"prev\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the previous page\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-learning-object-instance-list-response-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: LearningObjectInstanceListResponse
---
