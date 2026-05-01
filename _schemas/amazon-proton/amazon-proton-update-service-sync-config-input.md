---
description: UpdateServiceSyncConfigInput schema from Amazon Proton API
layout: schema
name: UpdateServiceSyncConfigInput
properties_list:
- description: ''
  name: branch
  type: object
- description: ''
  name: filePath
  type: object
- description: ''
  name: repositoryName
  type: object
- description: ''
  name: repositoryProvider
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-sync-config-input-schema.json
slug: amazon-proton-update-service-sync-config-input
source_filename: amazon-proton-update-service-sync-config-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-sync-config-input-schema.json\",\n  \"title\": \"UpdateServiceSyncConfigInput\",\n  \"description\": \"UpdateServiceSyncConfigInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The name of the code repository branch where the Proton Ops file is found.\"\n        }\n      ]\n    },\n    \"filePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpsFilePath\"\n        },\n        {\n          \"description\": \"The path to the Proton Ops file.\"\n        }\n      ]\n    },\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"The name of the repository where the Proton Ops file is found.\"\n        }\n      ]\n    },\n    \"repositoryProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The name of the repository provider where the Proton Ops file is found.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service the Proton Ops file is for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"branch\",\n    \"filePath\",\n    \"repositoryName\",\n    \"repositoryProvider\",\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-sync-config-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServiceSyncConfigInput
---
