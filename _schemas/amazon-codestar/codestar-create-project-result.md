---
description: CreateProjectResult schema from AWS CodeStar API
layout: schema
name: CreateProjectResult
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: projectTemplateId
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-create-project-result-schema.json
slug: codestar-create-project-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-create-project-result-schema.json\",\n  \"title\": \"CreateProjectResult\",\n  \"description\": \"CreateProjectResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the created project.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n      \
  \    \"description\": \"A user- or system-generated token that identifies the entity that requested project creation.\"\n        }\n      ]\n    },\n    \"projectTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectTemplateId\"\n        },\n        {\n          \"description\": \"Reserved for future use.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-create-project-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: CreateProjectResult
---
