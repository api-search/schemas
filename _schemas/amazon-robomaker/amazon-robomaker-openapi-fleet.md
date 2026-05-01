---
description: Information about a fleet.
layout: schema
name: Fleet
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
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
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-fleet-schema.json
slug: amazon-robomaker-openapi-fleet
source_filename: amazon-robomaker-openapi-fleet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-fleet-schema.json\",\n  \"title\": \"Fleet\",\n  \"description\": \"Information about a fleet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the fleet.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the\
  \ fleet was created.\"\n        }\n      ]\n    },\n    \"lastDeploymentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The status of the last fleet deployment.\"\n        }\n      ]\n    },\n    \"lastDeploymentJob\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the last deployment job.\"\n        }\n      ]\n    },\n    \"lastDeploymentTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time of the last deployment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-fleet-schema.json
tags:
- Robotics
- Simulation
title: Fleet
---
