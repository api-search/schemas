---
description: CreateTemplateSyncConfigInput schema from Amazon Proton API
layout: schema
name: CreateTemplateSyncConfigInput
properties_list:
- description: ''
  name: branch
  type: object
- description: ''
  name: repositoryName
  type: object
- description: ''
  name: repositoryProvider
  type: object
- description: ''
  name: subdirectory
  type: object
- description: ''
  name: templateName
  type: object
- description: ''
  name: templateType
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-template-sync-config-input-schema.json
slug: amazon-proton-create-template-sync-config-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-template-sync-config-input-schema.json\",\n  \"title\": \"CreateTemplateSyncConfigInput\",\n  \"description\": \"CreateTemplateSyncConfigInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The repository branch for your template.\"\n        }\n      ]\n    },\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"The repository name (for example, <code>myrepos/myrepo</code>).\"\n        }\n      ]\n    },\n    \"repositoryProvider\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The provider type for your repository.\"\n        }\n      ]\n    },\n    \"subdirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Subdirectory\"\n        },\n        {\n          \"description\": \"A repository subdirectory path to your template bundle directory. When included, Proton limits the template bundle search to this repository directory.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of your registered template.\"\n        }\n      ]\n    },\n    \"templateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The type of the registered template.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"branch\",\n    \"repositoryName\",\n    \"repositoryProvider\",\n    \"templateName\",\n    \"templateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-template-sync-config-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateTemplateSyncConfigInput
---
