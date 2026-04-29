---
description: Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: DeregisterRobotResponse
properties_list:
- description: ''
  name: fleet
  type: object
- description: ''
  name: robot
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-deregister-robot-response-schema.json
slug: amazon-robomaker-openapi-deregister-robot-response
source_filename: amazon-robomaker-openapi-deregister-robot-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-deregister-robot-response-schema.json\",\n  \"title\": \"DeregisterRobotResponse\",\n  \"description\": \"Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet.\"\n        }\n      ]\n    },\n    \"robot\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the robot.\"\n        }\n      ]\n    }\n  },\n  \"deprecated\"\
  : true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-deregister-robot-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DeregisterRobotResponse
---
