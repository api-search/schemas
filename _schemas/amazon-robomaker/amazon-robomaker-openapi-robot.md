---
description: Information about a robot.
layout: schema
name: Robot
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: fleetArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: greenGrassGroupId
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: architecture
  type: object
- description: ''
  name: lastDeploymentJob
  type: object
- description: ''
  name: lastDeploymentTime
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-robot-schema.json
slug: amazon-robomaker-openapi-robot
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-robot-schema.json\",\n  \"title\": \"Robot\",\n  \"description\": \"Information about a robot.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the robot.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the robot.\"\n        }\n      ]\n    },\n    \"fleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet.\"\n        }\n\
  \      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotStatus\"\n        },\n        {\n          \"description\": \"The status of the robot.\"\n        }\n      ]\n    },\n    \"greenGrassGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The Greengrass group associated with the robot.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the robot was created.\"\n        }\n      ]\n    },\n    \"architecture\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Architecture\"\n        },\n        {\n          \"description\": \"The architecture of the robot.\"\n        }\n      ]\n    },\n    \"lastDeploymentJob\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the last deployment job.\"\n        }\n      ]\n    },\n    \"lastDeploymentTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time of the last deployment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-robot-schema.json
tags:
- AWS
- Robotics
- Simulation
title: Robot
---
