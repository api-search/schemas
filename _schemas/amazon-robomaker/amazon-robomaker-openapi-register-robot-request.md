---
description: AWS RoboMaker is unable to process this request as the support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: RegisterRobotRequest
properties_list:
- description: ''
  name: fleet
  type: object
- description: ''
  name: robot
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-register-robot-request-schema.json
slug: amazon-robomaker-openapi-register-robot-request
source_filename: amazon-robomaker-openapi-register-robot-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-register-robot-request-schema.json\",\n  \"title\": \"RegisterRobotRequest\",\n  \"description\": \"AWS RoboMaker is unable to process this request as the support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the fleet.\"\n        }\n      ]\n    },\n    \"robot\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the robot.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fleet\",\n    \"robot\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-register-robot-request-schema.json
tags:
- Robotics
- Simulation
title: RegisterRobotRequest
---
