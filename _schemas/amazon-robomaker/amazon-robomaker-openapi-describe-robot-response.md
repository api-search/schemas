---
description: Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: DescribeRobotResponse
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
  name: greengrassGroupId
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
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-robot-response-schema.json
slug: amazon-robomaker-openapi-describe-robot-response
source_filename: amazon-robomaker-openapi-describe-robot-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-robot-response-schema.json\",\n  \"title\": \"DescribeRobotResponse\",\n  \"description\": \"Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the robot.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the robot.\"\n        }\n      ]\n    },\n    \"fleetArn\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotStatus\"\n        },\n        {\n          \"description\": \"The status of the fleet.\"\n        }\n      ]\n    },\n    \"greengrassGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The Greengrass group id.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the robot was created.\"\n        }\n      ]\n    },\n    \"architecture\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Architecture\"\
  \n        },\n        {\n          \"description\": \"The target architecture of the robot application.\"\n        }\n      ]\n    },\n    \"lastDeploymentJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the last deployment job.\"\n        }\n      ]\n    },\n    \"lastDeploymentTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time of the last deployment job.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of all tags added to the specified robot.\"\n        }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-robot-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DescribeRobotResponse
---
