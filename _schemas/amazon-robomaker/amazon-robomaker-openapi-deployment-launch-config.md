---
description: Configuration information for a deployment launch.
layout: schema
name: DeploymentLaunchConfig
properties_list:
- description: ''
  name: packageName
  type: object
- description: ''
  name: preLaunchFile
  type: object
- description: ''
  name: launchFile
  type: object
- description: ''
  name: postLaunchFile
  type: object
- description: ''
  name: environmentVariables
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-deployment-launch-config-schema.json
slug: amazon-robomaker-openapi-deployment-launch-config
source_filename: amazon-robomaker-openapi-deployment-launch-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-deployment-launch-config-schema.json\",\n  \"title\": \"DeploymentLaunchConfig\",\n  \"description\": \"Configuration information for a deployment launch.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Command\"\n        },\n        {\n          \"description\": \"The package name.\"\n        }\n      ]\n    },\n    \"preLaunchFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Path\"\n        },\n        {\n          \"description\": \"The deployment pre-launch file. This file will be executed prior to the launch file.\"\n        }\n      ]\n    },\n    \"launchFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Command\"\
  \n        },\n        {\n          \"description\": \"The launch file name.\"\n        }\n      ]\n    },\n    \"postLaunchFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Path\"\n        },\n        {\n          \"description\": \"The deployment post-launch file. This file will be executed after the launch file.\"\n        }\n      ]\n    },\n    \"environmentVariables\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentVariableMap\"\n        },\n        {\n          \"description\": \"An array of key/value pairs specifying environment variables for the robot application\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"packageName\",\n    \"launchFile\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-deployment-launch-config-schema.json
tags:
- Robotics
- Simulation
title: DeploymentLaunchConfig
---
