---
description: Contains information about policies that define how a deployment updates components and handles failure.
layout: schema
name: DeploymentPolicies
properties_list:
- description: ''
  name: failureHandlingPolicy
  type: object
- description: ''
  name: componentUpdatePolicy
  type: object
- description: ''
  name: configurationValidationPolicy
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-deployment-policies-schema.json
slug: iot-greengrass-deployment-policies
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-policies-schema.json\",\n  \"title\": \"DeploymentPolicies\",\n  \"description\": \"Contains information about policies that define how a deployment updates components and handles failure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failureHandlingPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentFailureHandlingPolicy\"\n        },\n        {\n          \"description\": \"<p>The failure handling policy for the configuration deployment. This policy defines what to do if the deployment fails.</p> <p>Default: <code>ROLLBACK</code> </p>\"\n        }\n      ]\n    },\n    \"componentUpdatePolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentComponentUpdatePolicy\"\n        },\n\
  \        {\n          \"description\": \"The component update policy for the configuration deployment. This policy defines when it's safe to deploy the configuration to devices.\"\n        }\n      ]\n    },\n    \"configurationValidationPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfigurationValidationPolicy\"\n        },\n        {\n          \"description\": \"The configuration validation policy for the configuration deployment. This policy defines how long each component has to validate its configure updates.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-policies-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DeploymentPolicies
---
