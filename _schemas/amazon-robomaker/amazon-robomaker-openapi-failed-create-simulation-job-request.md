---
description: Information about a failed create simulation job request.
layout: schema
name: FailedCreateSimulationJobRequest
properties_list:
- description: ''
  name: request
  type: object
- description: ''
  name: failureReason
  type: object
- description: ''
  name: failureCode
  type: object
- description: ''
  name: failedAt
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-failed-create-simulation-job-request-schema.json
slug: amazon-robomaker-openapi-failed-create-simulation-job-request
source_filename: amazon-robomaker-openapi-failed-create-simulation-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-failed-create-simulation-job-request-schema.json\",\n  \"title\": \"FailedCreateSimulationJobRequest\",\n  \"description\": \"Information about a failed create simulation job request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationJobRequest\"\n        },\n        {\n          \"description\": \"The simulation job request.\"\n        }\n      ]\n    },\n    \"failureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The failure reason of the simulation job request.\"\n        }\n      ]\n    },\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/SimulationJobErrorCode\"\n        },\n        {\n          \"description\": \"The failure code.\"\n        }\n      ]\n    },\n    \"failedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation job batch failed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-failed-create-simulation-job-request-schema.json
tags:
- Robotics
- Simulation
title: FailedCreateSimulationJobRequest
---
