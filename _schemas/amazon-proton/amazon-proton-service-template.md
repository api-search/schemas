---
description: Detailed data of an Proton service template resource.
layout: schema
name: ServiceTemplate
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: encryptionKey
  type: object
- description: ''
  name: lastModifiedAt
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: pipelineProvisioning
  type: object
- description: ''
  name: recommendedVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-service-template-schema.json
slug: amazon-proton-service-template
source_filename: amazon-proton-service-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-template-schema.json\",\n  \"title\": \"ServiceTemplate\",\n  \"description\": \"Detailed data of an Proton service template resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceTemplateArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the service template.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the service template was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n   \
  \     },\n        {\n          \"description\": \"A description of the service template.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayName\"\n        },\n        {\n          \"description\": \"The service template name as displayed in the developer interface.\"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The customer provided service template encryption key that's used to encrypt data.\"\n        }\n      ]\n    },\n    \"lastModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the service template was last modified.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\
  \n        },\n        {\n          \"description\": \"The name of the service template.\"\n        }\n      ]\n    },\n    \"pipelineProvisioning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Provisioning\"\n        },\n        {\n          \"description\": \"If <code>pipelineProvisioning</code> is <code>true</code>, a service pipeline is included in the service template. Otherwise, a service pipeline <i>isn't</i> included in the service template.\"\n        }\n      ]\n    },\n    \"recommendedVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FullTemplateVersionNumber\"\n        },\n        {\n          \"description\": \"The recommended version of the service template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"lastModifiedAt\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-template-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ServiceTemplate
---
