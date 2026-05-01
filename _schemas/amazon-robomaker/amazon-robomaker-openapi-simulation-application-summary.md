---
description: Summary information for a simulation application.
layout: schema
name: SimulationApplicationSummary
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: robotSoftwareSuite
  type: object
- description: ''
  name: simulationSoftwareSuite
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-simulation-application-summary-schema.json
slug: amazon-robomaker-openapi-simulation-application-summary
source_filename: amazon-robomaker-openapi-simulation-application-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-application-summary-schema.json\",\n  \"title\": \"SimulationApplicationSummary\",\n  \"description\": \"Summary information for a simulation application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the simulation application.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the simulation application.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n \
  \       },\n        {\n          \"description\": \"The version of the simulation application.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation application was last updated.\"\n        }\n      ]\n    },\n    \"robotSoftwareSuite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotSoftwareSuite\"\n        },\n        {\n          \"description\": \"Information about a robot software suite (ROS distribution).\"\n        }\n      ]\n    },\n    \"simulationSoftwareSuite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationSoftwareSuite\"\n        },\n        {\n          \"description\": \"Information about a simulation software suite.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-application-summary-schema.json
tags:
- Robotics
- Simulation
title: SimulationApplicationSummary
---
