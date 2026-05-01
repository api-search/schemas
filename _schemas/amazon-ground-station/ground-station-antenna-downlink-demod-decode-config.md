---
description: Information about how AWS Ground Station should conﬁgure an antenna for downlink demod decode during a contact.
layout: schema
name: AntennaDownlinkDemodDecodeConfig
properties_list:
- description: ''
  name: decodeConfig
  type: object
- description: ''
  name: demodulationConfig
  type: object
- description: ''
  name: spectrumConfig
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-antenna-downlink-demod-decode-config-schema.json
slug: ground-station-antenna-downlink-demod-decode-config
source_filename: ground-station-antenna-downlink-demod-decode-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-antenna-downlink-demod-decode-config-schema.json\",\n  \"title\": \"AntennaDownlinkDemodDecodeConfig\",\n  \"description\": \"Information about how AWS Ground Station should con\\ufb01gure an antenna for downlink demod decode during a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"decodeConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DecodeConfig\"\n        },\n        {\n          \"description\": \"Information about the decode <code>Config</code>.\"\n        }\n      ]\n    },\n    \"demodulationConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DemodulationConfig\"\n        },\n        {\n          \"description\": \"Information about the demodulation <code>Config</code>.\"\n        }\n\
  \      ]\n    },\n    \"spectrumConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpectrumConfig\"\n        },\n        {\n          \"description\": \"Information about the spectral <code>Config</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"decodeConfig\",\n    \"demodulationConfig\",\n    \"spectrumConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-antenna-downlink-demod-decode-config-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: AntennaDownlinkDemodDecodeConfig
---
