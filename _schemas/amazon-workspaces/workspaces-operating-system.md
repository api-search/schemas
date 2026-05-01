---
description: The operating system that the image is running.
layout: schema
name: OperatingSystem
properties_list:
- description: ''
  name: Type
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-operating-system-schema.json
slug: workspaces-operating-system
source_filename: workspaces-operating-system-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperatingSystemType\"\n        },\n        {\n          \"description\": \"The operating system.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The operating system that the image is running.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OperatingSystem\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-operating-system-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-operating-system-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: OperatingSystem
---
