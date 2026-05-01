---
description: Information about a robot deployment.
layout: schema
name: RobotDeployment
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: deploymentStartTime
  type: object
- description: ''
  name: deploymentFinishTime
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: progressDetail
  type: object
- description: ''
  name: failureReason
  type: object
- description: ''
  name: failureCode
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-robot-deployment-schema.json
slug: amazon-robomaker-openapi-robot-deployment
source_filename: amazon-robomaker-openapi-robot-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-robot-deployment-schema.json\",\n  \"title\": \"RobotDeployment\",\n  \"description\": \"Information about a robot deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The robot deployment Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"deploymentStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the deployment was started.\"\n        }\n      ]\n    },\n    \"deploymentFinishTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\
  \n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the deployment finished.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotStatus\"\n        },\n        {\n          \"description\": \"The status of the robot deployment.\"\n        }\n      ]\n    },\n    \"progressDetail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressDetail\"\n        },\n        {\n          \"description\": \"Information about how the deployment is progressing.\"\n        }\n      ]\n    },\n    \"failureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A short description of the reason why the robot deployment failed.\"\n        }\n      ]\n    },\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentJobErrorCode\"\
  \n        },\n        {\n          \"description\": \"The robot deployment failure code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-robot-deployment-schema.json
tags:
- Robotics
- Simulation
title: RobotDeployment
---
