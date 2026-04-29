---
description: Describes a WorkSpace modification.
layout: schema
name: ModificationState
properties_list:
- description: ''
  name: Resource
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modification-state-schema.json
slug: workspaces-modification-state
source_filename: workspaces-modification-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModificationResourceEnum\"\n        },\n        {\n          \"description\": \"The resource.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModificationStateEnum\"\n        },\n        {\n          \"description\": \"The modification state.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a WorkSpace modification.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModificationState\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modification-state-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modification-state-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModificationState
---
