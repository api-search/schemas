---
description: Summary information for a simulation job.
layout: schema
name: SimulationJobSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: simulationApplicationNames
  type: object
- description: ''
  name: robotApplicationNames
  type: object
- description: ''
  name: dataSourceNames
  type: object
- description: ''
  name: computeType
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-simulation-job-summary-schema.json
slug: amazon-robomaker-openapi-simulation-job-summary
source_filename: amazon-robomaker-openapi-simulation-job-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-job-summary-schema.json\",\n  \"title\": \"SimulationJobSummary\",\n  \"description\": \"Summary information for a simulation job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the simulation job.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation job was last updated.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\
  \n        },\n        {\n          \"description\": \"The name of the simulation job.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationJobStatus\"\n        },\n        {\n          \"description\": \"The status of the simulation job.\"\n        }\n      ]\n    },\n    \"simulationApplicationNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationApplicationNames\"\n        },\n        {\n          \"description\": \"A list of simulation job simulation application names.\"\n        }\n      ]\n    },\n    \"robotApplicationNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotApplicationNames\"\n        },\n        {\n          \"description\": \"A list of simulation job robot application names.\"\n        }\n      ]\n    },\n    \"dataSourceNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceNames\"\
  \n        },\n        {\n          \"description\": \"The names of the data sources.\"\n        }\n      ]\n    },\n    \"computeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeType\"\n        },\n        {\n          \"description\": \"The compute type for the simulation job summary.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-job-summary-schema.json
tags:
- AWS
- Robotics
- Simulation
title: SimulationJobSummary
---
