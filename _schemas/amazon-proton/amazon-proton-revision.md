---
description: Revision detail data for a commit and push that activates a sync attempt
layout: schema
name: Revision
properties_list:
- description: ''
  name: branch
  type: object
- description: ''
  name: directory
  type: object
- description: ''
  name: repositoryName
  type: object
- description: ''
  name: repositoryProvider
  type: object
- description: ''
  name: sha
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-revision-schema.json
slug: amazon-proton-revision
source_filename: amazon-proton-revision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-revision-schema.json\",\n  \"title\": \"Revision\",\n  \"description\": \"Revision detail data for a commit and push that activates a sync attempt\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The repository branch.\"\n        }\n      ]\n    },\n    \"directory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The repository directory changed by a commit and push that activated the sync attempt.\"\n        }\n      ]\n    },\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\
  \n        },\n        {\n          \"description\": \"The repository name.\"\n        }\n      ]\n    },\n    \"repositoryProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The repository provider.\"\n        }\n      ]\n    },\n    \"sha\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SHA\"\n        },\n        {\n          \"description\": \"The secure hash algorithm (SHA) hash for the revision.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"branch\",\n    \"directory\",\n    \"repositoryName\",\n    \"repositoryProvider\",\n    \"sha\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-revision-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: Revision
---
