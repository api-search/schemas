---
description: Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: DescribeRobotRequest
properties_list:
- description: ''
  name: robot
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-robot-request-schema.json
slug: amazon-robomaker-openapi-describe-robot-request
source_filename: amazon-robomaker-openapi-describe-robot-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-robot-request-schema.json\",\n  \"title\": \"DescribeRobotRequest\",\n  \"description\": \"Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"robot\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the robot to be described.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"robot\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-robot-request-schema.json
tags:
- Robotics
- Simulation
title: DescribeRobotRequest
---
