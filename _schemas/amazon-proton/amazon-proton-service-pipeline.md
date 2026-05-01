---
description: Detailed data of an Proton service instance pipeline resource.
layout: schema
name: ServicePipeline
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: deploymentStatus
  type: object
- description: ''
  name: deploymentStatusMessage
  type: object
- description: ''
  name: lastDeploymentAttemptedAt
  type: object
- description: ''
  name: lastDeploymentSucceededAt
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: templateMajorVersion
  type: object
- description: ''
  name: templateMinorVersion
  type: object
- description: ''
  name: templateName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-service-pipeline-schema.json
slug: amazon-proton-service-pipeline
source_filename: amazon-proton-service-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-pipeline-schema.json\",\n  \"title\": \"ServicePipeline\",\n  \"description\": \"Detailed data of an Proton service instance pipeline resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the service pipeline.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the service pipeline was created.\"\n        }\n      ]\n    },\n    \"deploymentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n\
  \        },\n        {\n          \"description\": \"The deployment status of the service pipeline.\"\n        }\n      ]\n    },\n    \"deploymentStatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"A service pipeline deployment status message.\"\n        }\n      ]\n    },\n    \"lastDeploymentAttemptedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when a deployment of the service pipeline was last attempted.\"\n        }\n      ]\n    },\n    \"lastDeploymentSucceededAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the service pipeline was last deployed successfully.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\": \"The service spec that was used to create the service pipeline.\"\n        }\n      ]\n    },\n    \"templateMajorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The major version of the service template that was used to create the service pipeline.\"\n        }\n      ]\n    },\n    \"templateMinorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The minor version of the service template that was used to create the service pipeline.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service template that\
  \ was used to create the service pipeline.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"deploymentStatus\",\n    \"lastDeploymentAttemptedAt\",\n    \"lastDeploymentSucceededAt\",\n    \"templateMajorVersion\",\n    \"templateMinorVersion\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-pipeline-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ServicePipeline
---
