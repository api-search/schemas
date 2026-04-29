---
description: Compute information for the simulation job
layout: schema
name: ComputeResponse
properties_list:
- description: ''
  name: simulationUnitLimit
  type: object
- description: ''
  name: computeType
  type: object
- description: ''
  name: gpuUnitLimit
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-compute-response-schema.json
slug: amazon-robomaker-openapi-compute-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-compute-response-schema.json\",\n  \"title\": \"ComputeResponse\",\n  \"description\": \"Compute information for the simulation job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"simulationUnitLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationUnit\"\n        },\n        {\n          \"description\": \"The simulation unit limit. Your simulation is allocated CPU and memory proportional to the supplied simulation unit limit. A simulation unit is 1 vcpu and 2GB of memory. You are only billed for the SU utilization you consume up to the maximum value provided. The default is 15. \"\n        }\n      ]\n    },\n    \"computeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeType\"\n     \
  \   },\n        {\n          \"description\": \"Compute type response information for the simulation job.\"\n        }\n      ]\n    },\n    \"gpuUnitLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GPUUnit\"\n        },\n        {\n          \"description\": \"Compute GPU unit limit for the simulation job. It is the same as the number of GPUs allocated to the SimulationJob.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-compute-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: ComputeResponse
---
