---
description: Object that describes a spectral <code>Config</code>.
layout: schema
name: SpectrumConfig
properties_list:
- description: ''
  name: bandwidth
  type: object
- description: ''
  name: centerFrequency
  type: object
- description: ''
  name: polarization
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-spectrum-config-schema.json
slug: ground-station-spectrum-config
source_filename: ground-station-spectrum-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-spectrum-config-schema.json\",\n  \"title\": \"SpectrumConfig\",\n  \"description\": \"Object that describes a spectral <code>Config</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bandwidth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrequencyBandwidth\"\n        },\n        {\n          \"description\": \"<p>Bandwidth of a spectral <code>Config</code>. AWS Ground Station currently has the following bandwidth limitations:</p> <ul> <li> <p>For <code>AntennaDownlinkDemodDecodeconfig</code>, valid values are between 125 kHz to 650 MHz.</p> </li> <li> <p>For <code>AntennaDownlinkconfig</code> valid values are between 10 kHz to 54 MHz.</p> </li> <li> <p>For <code>AntennaUplinkConfig</code>, valid values are between 10 kHz to 54 MHz.</p>\
  \ </li> </ul>\"\n        }\n      ]\n    },\n    \"centerFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Frequency\"\n        },\n        {\n          \"description\": \"Center frequency of a spectral <code>Config</code>. Valid values are between 2200 to 2300 MHz and 7750 to 8400 MHz for downlink and 2025 to 2120 MHz for uplink.\"\n        }\n      ]\n    },\n    \"polarization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Polarization\"\n        },\n        {\n          \"description\": \"Polarization of a spectral <code>Config</code>. Capturing both <code>\\\"RIGHT_HAND\\\"</code> and <code>\\\"LEFT_HAND\\\"</code> polarization requires two separate configs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bandwidth\",\n    \"centerFrequency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-spectrum-config-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: SpectrumConfig
---
