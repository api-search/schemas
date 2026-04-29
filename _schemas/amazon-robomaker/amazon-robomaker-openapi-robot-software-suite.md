---
description: Information about a robot software suite (ROS distribution).
layout: schema
name: RobotSoftwareSuite
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-robot-software-suite-schema.json
slug: amazon-robomaker-openapi-robot-software-suite
source_filename: amazon-robomaker-openapi-robot-software-suite-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-robot-software-suite-schema.json\",\n  \"title\": \"RobotSoftwareSuite\",\n  \"description\": \"Information about a robot software suite (ROS distribution).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotSoftwareSuiteType\"\n        },\n        {\n          \"description\": \"The name of the robot software suite (ROS distribution).\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotSoftwareSuiteVersionType\"\n        },\n        {\n          \"description\": \"The version of the robot software suite (ROS distribution).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-robot-software-suite-schema.json
tags:
- AWS
- Robotics
- Simulation
title: RobotSoftwareSuite
---
