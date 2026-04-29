---
description: A skill competency defined in the Learning Manager system
layout: schema
name: Skill
properties_list:
- description: Unique skill identifier
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: ''
  name: relationships
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-skill-schema.json
slug: prime-api-skill
source_filename: prime-api-skill-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-skill-schema.json\",\n  \"title\": \"Skill\",\n  \"description\": \"A skill competency defined in the Learning Manager system\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique skill identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"skill\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Skill description\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Skill name\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Skill state\",\n          \"enum\": [\n        \
  \    \"Active\",\n            \"Retired\"\n          ]\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"skillLevels\": {\n          \"type\": \"object\",\n          \"description\": \"A JSON:API relationship object\",\n          \"properties\": {\n            \"data\": {\n              \"oneOf\": [\n                {\n                  \"type\": \"object\",\n                  \"description\": \"JSON:API resource identifier\",\n                  \"required\": [\n                    \"id\",\n                    \"type\"\n                  ],\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"string\",\n                      \"description\": \"Resource identifier\"\n                    },\n                    \"type\": {\n                      \"type\": \"string\",\n                      \"description\": \"Resource type name\"\n                    }\n                 \
  \ }\n                },\n                {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"description\": \"JSON:API resource identifier\",\n                    \"required\": [\n                      \"id\",\n                      \"type\"\n                    ],\n                    \"properties\": {\n                      \"id\": {\n                        \"type\": \"string\",\n                        \"description\": \"Resource identifier\"\n                      },\n                      \"type\": {\n                        \"type\": \"string\",\n                        \"description\": \"Resource type name\"\n                      }\n                    }\n                  }\n                }\n              ]\n            },\n            \"links\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"related\": {\n                  \"type\": \"string\"\
  ,\n                  \"format\": \"uri\",\n                  \"description\": \"URL to fetch the related resource\"\n                }\n              }\n            }\n          }\n        },\n        \"learningObjects\": {\n          \"type\": \"object\",\n          \"description\": \"A JSON:API relationship object\",\n          \"properties\": {\n            \"data\": {\n              \"oneOf\": [\n                {\n                  \"type\": \"object\",\n                  \"description\": \"JSON:API resource identifier\",\n                  \"required\": [\n                    \"id\",\n                    \"type\"\n                  ],\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"string\",\n                      \"description\": \"Resource identifier\"\n                    },\n                    \"type\": {\n                      \"type\": \"string\",\n                      \"description\": \"Resource type name\"\n       \
  \             }\n                  }\n                },\n                {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"description\": \"JSON:API resource identifier\",\n                    \"required\": [\n                      \"id\",\n                      \"type\"\n                    ],\n                    \"properties\": {\n                      \"id\": {\n                        \"type\": \"string\",\n                        \"description\": \"Resource identifier\"\n                      },\n                      \"type\": {\n                        \"type\": \"string\",\n                        \"description\": \"Resource type name\"\n                      }\n                    }\n                  }\n                }\n              ]\n            },\n            \"links\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"related\": {\n    \
  \              \"type\": \"string\",\n                  \"format\": \"uri\",\n                  \"description\": \"URL to fetch the related resource\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-skill-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: Skill
---
