---
description: CreateConnectionAliasResult schema from Amazon WorkSpaces API
layout: schema
name: CreateConnectionAliasResult
properties_list:
- description: ''
  name: AliasId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-connection-alias-result-schema.json
slug: workspaces-create-connection-alias-result
source_filename: workspaces-create-connection-alias-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasId\"\n        },\n        {\n          \"description\": \"The identifier of the connection alias.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateConnectionAliasResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-connection-alias-result-schema.json\",\n  \"description\": \"CreateConnectionAliasResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-connection-alias-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateConnectionAliasResult
---
