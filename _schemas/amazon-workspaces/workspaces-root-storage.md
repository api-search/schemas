---
description: Describes the root volume for a WorkSpace bundle.
layout: schema
name: RootStorage
properties_list:
- description: ''
  name: Capacity
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-root-storage-schema.json
slug: workspaces-root-storage
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Capacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The size of the root volume.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the root volume for a WorkSpace bundle.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RootStorage\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-root-storage-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-root-storage-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: RootStorage
---
