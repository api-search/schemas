---
description: Information about the uplink spectral <code>Config</code>.
layout: schema
name: UplinkSpectrumConfig
properties_list:
- description: ''
  name: centerFrequency
  type: object
- description: ''
  name: polarization
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-uplink-spectrum-config-schema.json
slug: ground-station-uplink-spectrum-config
source_filename: ground-station-uplink-spectrum-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-uplink-spectrum-config-schema.json\",\n  \"title\": \"UplinkSpectrumConfig\",\n  \"description\": \"Information about the uplink spectral <code>Config</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"centerFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Frequency\"\n        },\n        {\n          \"description\": \"Center frequency of an uplink spectral <code>Config</code>. Valid values are between 2025 to 2120 MHz.\"\n        }\n      ]\n    },\n    \"polarization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Polarization\"\n        },\n        {\n          \"description\": \"Polarization of an uplink spectral <code>Config</code>. Capturing both <code>\\\"RIGHT_HAND\\\"</code> and <code>\\\
  \"LEFT_HAND\\\"</code> polarization requires two separate configs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"centerFrequency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-uplink-spectrum-config-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: UplinkSpectrumConfig
---
