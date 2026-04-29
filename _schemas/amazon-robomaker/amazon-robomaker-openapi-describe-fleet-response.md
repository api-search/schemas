---
description: Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: DescribeFleetResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: robots
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: lastDeploymentStatus
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
schema_file: json-schema/amazon-robomaker-openapi-describe-fleet-response-schema.json
slug: amazon-robomaker-openapi-describe-fleet-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-fleet-response-schema.json\",\n  \"title\": \"DescribeFleetResponse\",\n  \"description\": \"Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the fleet.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet.\"\n        }\n      ]\n    },\n    \"robots\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/Robots\"\n        },\n        {\n          \"description\": \"A list of robots.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the fleet was created.\"\n        }\n      ]\n    },\n    \"lastDeploymentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The status of the last deployment.\"\n        }\n      ]\n    },\n    \"lastDeploymentJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the last deployment job.\"\n        }\n      ]\n    },\n    \"lastDeploymentTime\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time of the last deployment.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of all tags added to the specified fleet.\"\n        }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-fleet-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DescribeFleetResponse
---
