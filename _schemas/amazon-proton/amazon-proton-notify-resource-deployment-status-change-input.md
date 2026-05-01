---
description: NotifyResourceDeploymentStatusChangeInput schema from Amazon Proton API
layout: schema
name: NotifyResourceDeploymentStatusChangeInput
properties_list:
- description: ''
  name: deploymentId
  type: object
- description: ''
  name: outputs
  type: object
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-notify-resource-deployment-status-change-input-schema.json
slug: amazon-proton-notify-resource-deployment-status-change-input
source_filename: amazon-proton-notify-resource-deployment-status-change-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-notify-resource-deployment-status-change-input-schema.json\",\n  \"title\": \"NotifyResourceDeploymentStatusChangeInput\",\n  \"description\": \"NotifyResourceDeploymentStatusChangeInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentId\"\n        },\n        {\n          \"description\": \"The deployment ID for your provisioned resource.\"\n        }\n      ]\n    },\n    \"outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotifyResourceDeploymentStatusChangeInputOutputsList\"\n        },\n        {\n          \"description\": \"The provisioned resource state change detail data that's returned by Proton.\"\n    \
  \    }\n      ]\n    },\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The provisioned resource Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceDeploymentStatus\"\n        },\n        {\n          \"description\": \"The status of your provisioned resource.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotifyResourceDeploymentStatusChangeInputStatusMessageString\"\n        },\n        {\n          \"description\": \"The deployment status message for your provisioned resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-notify-resource-deployment-status-change-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: NotifyResourceDeploymentStatusChangeInput
---
