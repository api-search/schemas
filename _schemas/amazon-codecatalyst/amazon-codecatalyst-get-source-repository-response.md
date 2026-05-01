---
description: GetSourceRepositoryResponse schema from Amazon CodeCatalyst
layout: schema
name: GetSourceRepositoryResponse
properties_list:
- description: ''
  name: spaceName
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: lastUpdatedTime
  type: object
- description: ''
  name: createdTime
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-get-source-repository-response-schema.json
slug: amazon-codecatalyst-get-source-repository-response
source_filename: amazon-codecatalyst-get-source-repository-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-source-repository-response-schema.json\",\n  \"title\": \"GetSourceRepositoryResponse\",\n  \"description\": \"GetSourceRepositoryResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryNameString\"\
  \n        },\n        {\n          \"description\": \"The name of the source repository.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryDescriptionString\"\n        },\n        {\n          \"description\": \"The description of the source repository.\"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the source repository was last updated, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    },\n    \"createdTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the source repository was created, in coordinated universal\
  \ time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spaceName\",\n    \"projectName\",\n    \"name\",\n    \"lastUpdatedTime\",\n    \"createdTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-source-repository-response-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: GetSourceRepositoryResponse
---
