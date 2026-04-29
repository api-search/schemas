---
description: Information about how AWS Ground Station should configure an antenna for downlink during a contact.
layout: schema
name: AntennaDownlinkConfig
properties_list:
- description: ''
  name: spectrumConfig
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-antenna-downlink-config-schema.json
slug: ground-station-antenna-downlink-config
source_filename: ground-station-antenna-downlink-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-antenna-downlink-config-schema.json\",\n  \"title\": \"AntennaDownlinkConfig\",\n  \"description\": \"Information about how AWS Ground Station should configure an antenna for downlink during a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spectrumConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpectrumConfig\"\n        },\n        {\n          \"description\": \"Object that describes a spectral <code>Config</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spectrumConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-antenna-downlink-config-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: AntennaDownlinkConfig
---
