---
description: Version information for agent components.
layout: schema
name: ComponentVersion
properties_list:
- description: ''
  name: componentType
  type: object
- description: ''
  name: versions
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-component-version-schema.json
slug: ground-station-component-version
source_filename: ground-station-component-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-component-version-schema.json\",\n  \"title\": \"ComponentVersion\",\n  \"description\": \"Version information for agent components.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentTypeString\"\n        },\n        {\n          \"description\": \"Component type.\"\n        }\n      ]\n    },\n    \"versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionStringList\"\n        },\n        {\n          \"description\": \"List of versions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"componentType\",\n    \"versions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-component-version-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ComponentVersion
---
