---
description: Describes the user volume for a WorkSpace bundle.
layout: schema
name: UserStorage
properties_list:
- description: ''
  name: Capacity
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-user-storage-schema.json
slug: workspaces-user-storage
source_filename: workspaces-user-storage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Capacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The size of the user volume.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the user volume for a WorkSpace bundle.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserStorage\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-user-storage-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-user-storage-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: UserStorage
---
