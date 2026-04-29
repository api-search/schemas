---
description: Summary data of an Proton service instance resource.
layout: schema
name: ServiceInstanceSummary
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
  name: environmentName
  type: object
- description: ''
  name: lastDeploymentAttemptedAt
  type: object
- description: ''
  name: lastDeploymentSucceededAt
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: serviceName
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
schema_file: json-schema/amazon-proton-service-instance-summary-schema.json
slug: amazon-proton-service-instance-summary
source_filename: amazon-proton-service-instance-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-instance-summary-schema.json\",\n  \"title\": \"ServiceInstanceSummary\",\n  \"description\": \"Summary data of an Proton service instance resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceInstanceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the service instance.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the service instance was created.\"\n        }\n      ]\n    },\n    \"deploymentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\
  \n        },\n        {\n          \"description\": \"The service instance deployment status.\"\n        }\n      ]\n    },\n    \"deploymentStatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"A service instance deployment status message.\"\n        }\n      ]\n    },\n    \"environmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment that the service instance was deployed into.\"\n        }\n      ]\n    },\n    \"lastDeploymentAttemptedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when a deployment of the service was last attempted.\"\n        }\n      ]\n    },\n    \"lastDeploymentSucceededAt\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the service was last deployed successfully.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service instance.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that the service instance belongs to.\"\n        }\n      ]\n    },\n    \"templateMajorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The service instance template major version.\"\n        }\n      ]\n    },\n    \"templateMinorVersion\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/TemplateVersionPart\"\n        },\n        {\n          \"description\": \"The service instance template minor version.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"createdAt\",\n    \"deploymentStatus\",\n    \"environmentName\",\n    \"lastDeploymentAttemptedAt\",\n    \"lastDeploymentSucceededAt\",\n    \"name\",\n    \"serviceName\",\n    \"templateMajorVersion\",\n    \"templateMinorVersion\",\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-service-instance-summary-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ServiceInstanceSummary
---
