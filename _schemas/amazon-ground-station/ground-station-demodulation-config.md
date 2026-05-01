---
description: Information about the demodulation <code>Config</code>.
layout: schema
name: DemodulationConfig
properties_list:
- description: ''
  name: unvalidatedJSON
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-demodulation-config-schema.json
slug: ground-station-demodulation-config
source_filename: ground-station-demodulation-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-demodulation-config-schema.json\",\n  \"title\": \"DemodulationConfig\",\n  \"description\": \"Information about the demodulation <code>Config</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unvalidatedJSON\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JsonString\"\n        },\n        {\n          \"description\": \"Unvalidated JSON of a demodulation <code>Config</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"unvalidatedJSON\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-demodulation-config-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: DemodulationConfig
---
