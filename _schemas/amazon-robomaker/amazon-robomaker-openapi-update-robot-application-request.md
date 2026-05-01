---
description: UpdateRobotApplicationRequest schema from openapi
layout: schema
name: UpdateRobotApplicationRequest
properties_list:
- description: ''
  name: application
  type: object
- description: ''
  name: sources
  type: object
- description: ''
  name: robotSoftwareSuite
  type: object
- description: ''
  name: currentRevisionId
  type: object
- description: ''
  name: environment
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-update-robot-application-request-schema.json
slug: amazon-robomaker-openapi-update-robot-application-request
source_filename: amazon-robomaker-openapi-update-robot-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-update-robot-application-request-schema.json\",\n  \"title\": \"UpdateRobotApplicationRequest\",\n  \"description\": \"UpdateRobotApplicationRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The application information for the robot application.\"\n        }\n      ]\n    },\n    \"sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceConfigs\"\n        },\n        {\n          \"description\": \"The sources of the robot application.\"\n        }\n      ]\n    },\n    \"robotSoftwareSuite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotSoftwareSuite\"\
  \n        },\n        {\n          \"description\": \"The robot software suite (ROS distribution) used by the robot application.\"\n        }\n      ]\n    },\n    \"currentRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \"The revision id for the robot application.\"\n        }\n      ]\n    },\n    \"environment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Environment\"\n        },\n        {\n          \"description\": \"The object that contains the Docker image URI for your robot application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"application\",\n    \"robotSoftwareSuite\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-update-robot-application-request-schema.json
tags:
- Robotics
- Simulation
title: UpdateRobotApplicationRequest
---
