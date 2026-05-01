---
description: Information about a source repository returned in a list of source repositories.
layout: schema
name: ListSourceRepositoriesItem
properties_list:
- description: ''
  name: id
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
schema_file: json-schema/amazon-codecatalyst-list-source-repositories-item-schema.json
slug: amazon-codecatalyst-list-source-repositories-item
source_filename: amazon-codecatalyst-list-source-repositories-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repositories-item-schema.json\",\n  \"title\": \"ListSourceRepositoriesItem\",\n  \"description\": \"Information about a source repository returned in a list of source repositories.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryIdString\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the source repository.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryNameString\"\n        },\n        {\n          \"description\": \"The name of the source repository.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/SourceRepositoryDescriptionString\"\n        },\n        {\n          \"description\": \"The description of the repository, if any.\"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the source repository was last updated, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    },\n    \"createdTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the source repository was created, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    }\n \
  \ },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"lastUpdatedTime\",\n    \"createdTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repositories-item-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ListSourceRepositoriesItem
---
