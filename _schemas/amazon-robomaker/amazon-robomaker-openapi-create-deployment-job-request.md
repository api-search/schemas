---
description: AWS RoboMaker is unable to process this request as the support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: CreateDeploymentJobRequest
properties_list:
- description: ''
  name: deploymentConfig
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: fleet
  type: object
- description: ''
  name: deploymentApplicationConfigs
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-create-deployment-job-request-schema.json
slug: amazon-robomaker-openapi-create-deployment-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-deployment-job-request-schema.json\",\n  \"title\": \"CreateDeploymentJobRequest\",\n  \"description\": \"AWS RoboMaker is unable to process this request as the support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deploymentConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfig\"\n        },\n        {\n          \"description\": \"The requested deployment configuration.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n       \
  \   \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"fleet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet to deploy.\"\n        }\n      ]\n    },\n    \"deploymentApplicationConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentApplicationConfigs\"\n        },\n        {\n          \"description\": \"The deployment application configuration.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the deployment job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"clientRequestToken\",\n    \"fleet\",\n    \"\
  deploymentApplicationConfigs\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-deployment-job-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: CreateDeploymentJobRequest
---
