---
description: Information about a simulation software suite.
layout: schema
name: SimulationSoftwareSuite
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-simulation-software-suite-schema.json
slug: amazon-robomaker-openapi-simulation-software-suite
source_filename: amazon-robomaker-openapi-simulation-software-suite-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-software-suite-schema.json\",\n  \"title\": \"SimulationSoftwareSuite\",\n  \"description\": \"Information about a simulation software suite.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationSoftwareSuiteType\"\n        },\n        {\n          \"description\": \"The name of the simulation software suite.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationSoftwareSuiteVersionType\"\n        },\n        {\n          \"description\": \"The version of the simulation software suite.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-software-suite-schema.json
tags:
- Robotics
- Simulation
title: SimulationSoftwareSuite
---
