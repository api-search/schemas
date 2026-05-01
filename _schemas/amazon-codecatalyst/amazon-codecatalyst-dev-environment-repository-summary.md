---
description: Information about the source repsitory for a Dev Environment.
layout: schema
name: DevEnvironmentRepositorySummary
properties_list:
- description: ''
  name: repositoryName
  type: object
- description: ''
  name: branchName
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-dev-environment-repository-summary-schema.json
slug: amazon-codecatalyst-dev-environment-repository-summary
source_filename: amazon-codecatalyst-dev-environment-repository-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-repository-summary-schema.json\",\n  \"title\": \"DevEnvironmentRepositorySummary\",\n  \"description\": \"Information about the source repsitory for a Dev Environment. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryNameString\"\n        },\n        {\n          \"description\": \"The name of the source repository.\"\n        }\n      ]\n    },\n    \"branchName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryBranchString\"\n        },\n        {\n          \"description\": \"The name of the branch in a source repository cloned into the Dev Environment. \"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"repositoryName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-repository-summary-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: DevEnvironmentRepositorySummary
---
