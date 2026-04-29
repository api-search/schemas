---
description: Status information about the simulation clock.
layout: schema
name: SimulationClock
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: TargetStatus
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-simulation-clock-schema.json
slug: amazon-simspace-weaver-simulation-clock
source_filename: amazon-simspace-weaver-simulation-clock-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-clock-schema.json\",\n  \"title\": \"SimulationClock\",\n  \"description\": \"Status information about the simulation clock.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClockStatus\"\n        },\n        {\n          \"description\": \"The current status of the simulation clock.\"\n        }\n      ]\n    },\n    \"TargetStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClockTargetStatus\"\n        },\n        {\n          \"description\": \"The desired status of the simulation clock.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-clock-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: SimulationClock
---
