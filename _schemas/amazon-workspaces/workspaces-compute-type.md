---
description: Describes the compute type of the bundle.
layout: schema
name: ComputeType
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-compute-type-schema.json
slug: workspaces-compute-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compute\"\n        },\n        {\n          \"description\": \"The compute type.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the compute type of the bundle.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComputeType\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-compute-type-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-compute-type-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ComputeType
---
