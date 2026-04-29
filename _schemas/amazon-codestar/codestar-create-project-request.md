---
description: CreateProjectRequest schema from AWS CodeStar API
layout: schema
name: CreateProjectRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: sourceCode
  type: object
- description: ''
  name: toolchain
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-create-project-request-schema.json
slug: codestar-create-project-request
source_filename: codestar-create-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-create-project-request-schema.json\",\n  \"title\": \"CreateProjectRequest\",\n  \"description\": \"CreateProjectRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The display name for the project to be created in AWS CodeStar.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project to be created in AWS CodeStar.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectDescription\"\
  \n        },\n        {\n          \"description\": \"The description of the project, if any.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"A user- or system-generated token that identifies the entity that requested project creation. This token can be used to repeat the request.\"\n        }\n      ]\n    },\n    \"sourceCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceCode\"\n        },\n        {\n          \"description\": \"A list of the Code objects submitted with the project request. If this parameter is specified, the request must also include the toolchain parameter.\"\n        }\n      ]\n    },\n    \"toolchain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Toolchain\"\n        },\n        {\n          \"description\": \"The name of the toolchain\
  \ template file submitted with the project request. If this parameter is specified, the request must also include the sourceCode parameter.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The tags created for the project.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-create-project-request-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: CreateProjectRequest
---
