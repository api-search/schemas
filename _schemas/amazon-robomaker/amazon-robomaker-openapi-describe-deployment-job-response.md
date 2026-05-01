---
description: Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: DescribeDeploymentJobResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: fleet
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: deploymentConfig
  type: object
- description: ''
  name: deploymentApplicationConfigs
  type: object
- description: ''
  name: failureReason
  type: object
- description: ''
  name: failureCode
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: robotDeploymentSummary
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-deployment-job-response-schema.json
slug: amazon-robomaker-openapi-describe-deployment-job-response
source_filename: amazon-robomaker-openapi-describe-deployment-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-deployment-job-response-schema.json\",\n  \"title\": \"DescribeDeploymentJobResponse\",\n  \"description\": \"Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the deployment job.\"\n        }\n      ]\n    },\n    \"fleet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet.\"\n        }\n      ]\n\
  \    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The status of the deployment job.\"\n        }\n      ]\n    },\n    \"deploymentConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfig\"\n        },\n        {\n          \"description\": \"The deployment configuration.\"\n        }\n      ]\n    },\n    \"deploymentApplicationConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentApplicationConfigs\"\n        },\n        {\n          \"description\": \"The deployment application configuration.\"\n        }\n      ]\n    },\n    \"failureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A short description of the reason why the deployment job failed.\"\n        }\n    \
  \  ]\n    },\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentJobErrorCode\"\n        },\n        {\n          \"description\": \"The deployment job failure code.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the deployment job was created.\"\n        }\n      ]\n    },\n    \"robotDeploymentSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotDeploymentSummary\"\n        },\n        {\n          \"description\": \"A list of robot deployment summaries.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of all tags added to the specified deployment job.\"\n \
  \       }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-deployment-job-response-schema.json
tags:
- Robotics
- Simulation
title: DescribeDeploymentJobResponse
---
