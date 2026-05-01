---
description: AWS RoboMaker is unable to process this request as the support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: RegisterRobotResponse
properties_list:
- description: ''
  name: fleet
  type: object
- description: ''
  name: robot
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-register-robot-response-schema.json
slug: amazon-robomaker-openapi-register-robot-response
source_filename: amazon-robomaker-openapi-register-robot-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-register-robot-response-schema.json\",\n  \"title\": \"RegisterRobotResponse\",\n  \"description\": \"AWS RoboMaker is unable to process this request as the support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet that the robot will join.\"\n        }\n      ]\n    },\n    \"robot\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"Information\
  \ about the robot registration.\"\n        }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-register-robot-response-schema.json
tags:
- Robotics
- Simulation
title: RegisterRobotResponse
---
