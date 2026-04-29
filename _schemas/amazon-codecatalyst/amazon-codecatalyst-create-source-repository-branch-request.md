---
description: CreateSourceRepositoryBranchRequest schema from Amazon CodeCatalyst
layout: schema
name: CreateSourceRepositoryBranchRequest
properties_list:
- description: ''
  name: headCommitId
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-source-repository-branch-request-schema.json
slug: amazon-codecatalyst-create-source-repository-branch-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-source-repository-branch-request-schema.json\",\n  \"title\": \"CreateSourceRepositoryBranchRequest\",\n  \"description\": \"CreateSourceRepositoryBranchRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"headCommitId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The commit ID in an existing branch from which you want to create the new branch.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-source-repository-branch-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateSourceRepositoryBranchRequest
---
