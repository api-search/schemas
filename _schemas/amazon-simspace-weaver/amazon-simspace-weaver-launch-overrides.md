---
description: Options that apply when the app starts. These options override default behavior.
layout: schema
name: LaunchOverrides
properties_list:
- description: ''
  name: LaunchCommands
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-launch-overrides-schema.json
slug: amazon-simspace-weaver-launch-overrides
source_filename: amazon-simspace-weaver-launch-overrides-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-launch-overrides-schema.json\",\n  \"title\": \"LaunchOverrides\",\n  \"description\": \"Options that apply when the app starts. These options override default behavior.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchCommands\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchCommandList\"\n        },\n        {\n          \"description\": \"App launch commands and command line parameters that override the launch command configured in the simulation schema.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-launch-overrides-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: LaunchOverrides
---
