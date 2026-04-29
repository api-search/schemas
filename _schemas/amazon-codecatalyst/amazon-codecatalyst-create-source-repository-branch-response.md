---
description: CreateSourceRepositoryBranchResponse schema from Amazon CodeCatalyst
layout: schema
name: CreateSourceRepositoryBranchResponse
properties_list:
- description: ''
  name: ref
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: lastUpdatedTime
  type: object
- description: ''
  name: headCommitId
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-source-repository-branch-response-schema.json
slug: amazon-codecatalyst-create-source-repository-branch-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-source-repository-branch-response-schema.json\",\n  \"title\": \"CreateSourceRepositoryBranchResponse\",\n  \"description\": \"CreateSourceRepositoryBranchResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ref\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryBranchRefString\"\n        },\n        {\n          \"description\": \"The Git reference name of the branch.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryBranchString\"\n        },\n        {\n          \"description\": \"The name of the newly created branch.\"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The time the branch was last updated, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    },\n    \"headCommitId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The commit ID of the tip of the newly created branch.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-source-repository-branch-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateSourceRepositoryBranchResponse
---
