---
description: StopSimulationInput schema from Amazon SimSpace Weaver API
layout: schema
name: StopSimulationInput
properties_list:
- description: ''
  name: Simulation
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-stop-simulation-input-schema.json
slug: amazon-simspace-weaver-stop-simulation-input
source_filename: amazon-simspace-weaver-stop-simulation-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-stop-simulation-input-schema.json\",\n  \"title\": \"StopSimulationInput\",\n  \"description\": \"StopSimulationInput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Simulation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the simulation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Simulation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-stop-simulation-input-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: StopSimulationInput
---
