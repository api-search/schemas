---
description: Information about a branch of a source repository returned in a list of branches.
layout: schema
name: ListSourceRepositoryBranchesItem
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
schema_file: json-schema/amazon-codecatalyst-list-source-repository-branches-item-schema.json
slug: amazon-codecatalyst-list-source-repository-branches-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repository-branches-item-schema.json\",\n  \"title\": \"ListSourceRepositoryBranchesItem\",\n  \"description\": \"Information about a branch of a source repository returned in a list of branches.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ref\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryBranchRefString\"\n        },\n        {\n          \"description\": \"The Git reference name of the branch.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryBranchString\"\n        },\n        {\n          \"description\": \"The name of the branch.\"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The time the branch was last updated, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a>.\"\n        }\n      ]\n    },\n    \"headCommitId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The commit ID of the tip of the branch at the time of the request, also known as the head commit.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repository-branches-item-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ListSourceRepositoryBranchesItem
---
