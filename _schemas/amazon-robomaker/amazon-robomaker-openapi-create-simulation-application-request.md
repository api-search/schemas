---
description: CreateSimulationApplicationRequest schema from openapi
layout: schema
name: CreateSimulationApplicationRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: sources
  type: object
- description: ''
  name: simulationSoftwareSuite
  type: object
- description: ''
  name: robotSoftwareSuite
  type: object
- description: ''
  name: renderingEngine
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: environment
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-create-simulation-application-request-schema.json
slug: amazon-robomaker-openapi-create-simulation-application-request
source_filename: amazon-robomaker-openapi-create-simulation-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-simulation-application-request-schema.json\",\n  \"title\": \"CreateSimulationApplicationRequest\",\n  \"description\": \"CreateSimulationApplicationRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the simulation application.\"\n        }\n      ]\n    },\n    \"sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceConfigs\"\n        },\n        {\n          \"description\": \"The sources of the simulation application.\"\n        }\n      ]\n    },\n    \"simulationSoftwareSuite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationSoftwareSuite\"\
  \n        },\n        {\n          \"description\": \"The simulation software suite used by the simulation application.\"\n        }\n      ]\n    },\n    \"robotSoftwareSuite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotSoftwareSuite\"\n        },\n        {\n          \"description\": \"The robot software suite (ROS distribution) used by the simulation application.\"\n        }\n      ]\n    },\n    \"renderingEngine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenderingEngine\"\n        },\n        {\n          \"description\": \"The rendering engine for the simulation application.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the simulation application.\"\n        }\n      ]\n    },\n    \"environment\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Environment\"\n        },\n        {\n          \"description\": \"The object that contains the Docker image URI used to create your simulation application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"simulationSoftwareSuite\",\n    \"robotSoftwareSuite\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-simulation-application-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: CreateSimulationApplicationRequest
---
