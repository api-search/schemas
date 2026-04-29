---
description: ''
layout: schema
name: TargetWorkspace
properties_list:
- description: ''
  name: targetWorkspace
  type: object
- description: The ttl for the item, in seconds. If not set, the default will be the target workspace ttl.
  name: ttl
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-target-workspace-schema.json
slug: oneatlas-target-workspace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-target-workspace-schema.json\",\n  \"title\": \"TargetWorkspace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetWorkspace\": {\n      \"$ref\": \"#/components/schemas/WorkspaceIdentifier\"\n    },\n    \"ttl\": {\n      \"description\": \"The ttl for the item, in seconds. If not set, the default will be the target workspace ttl.\",\n      \"example\": 123456,\n      \"format\": \"int\",\n      \"minimum\": 1,\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-target-workspace-schema.json
tags:
- Imagery
- Satellites
title: TargetWorkspace
---
