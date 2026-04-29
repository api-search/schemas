---
description: Request body for creating an enrollment
layout: schema
name: EnrollmentCreateRequest
properties_list:
- description: ''
  name: data
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-enrollment-create-request-schema.json
slug: prime-api-enrollment-create-request
source_filename: prime-api-enrollment-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-enrollment-create-request-schema.json\",\n  \"title\": \"EnrollmentCreateRequest\",\n  \"description\": \"Request body for creating an enrollment\",\n  \"type\": \"object\",\n  \"required\": [\n    \"data\"\n  ],\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"type\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"enrollment\"\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"loInstanceId\": {\n              \"type\": \"string\",\n              \"description\": \"ID of the learning object instance to enroll in\"\n            }\n          }\n        },\n        \"relationships\": {\n    \
  \      \"type\": \"object\",\n          \"properties\": {\n            \"loInstance\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"data\": {\n                  \"type\": \"object\",\n                  \"description\": \"JSON:API resource identifier\",\n                  \"required\": [\n                    \"id\",\n                    \"type\"\n                  ],\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"string\",\n                      \"description\": \"Resource identifier\"\n                    },\n                    \"type\": {\n                      \"type\": \"string\",\n                      \"description\": \"Resource type name\"\n                    }\n                  }\n                }\n              }\n            },\n            \"learner\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"data\": {\n                  \"\
  type\": \"object\",\n                  \"description\": \"JSON:API resource identifier\",\n                  \"required\": [\n                    \"id\",\n                    \"type\"\n                  ],\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"string\",\n                      \"description\": \"Resource identifier\"\n                    },\n                    \"type\": {\n                      \"type\": \"string\",\n                      \"description\": \"Resource type name\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-enrollment-create-request-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: EnrollmentCreateRequest
---
