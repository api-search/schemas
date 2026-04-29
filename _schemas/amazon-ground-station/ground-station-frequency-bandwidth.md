---
description: Object that describes the frequency bandwidth.
layout: schema
name: FrequencyBandwidth
properties_list:
- description: ''
  name: units
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-frequency-bandwidth-schema.json
slug: ground-station-frequency-bandwidth
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-frequency-bandwidth-schema.json\",\n  \"title\": \"FrequencyBandwidth\",\n  \"description\": \"Object that describes the frequency bandwidth. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"units\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BandwidthUnits\"\n        },\n        {\n          \"description\": \"Frequency bandwidth units.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"<p>Frequency bandwidth value. AWS Ground Station currently has the following bandwidth limitations:</p> <ul> <li> <p>For <code>AntennaDownlinkDemodDecodeconfig</code>, valid values are between 125 kHz to 650 MHz.</p> </li> <li>\
  \ <p>For <code>AntennaDownlinkconfig</code>, valid values are between 10 kHz to 54 MHz.</p> </li> <li> <p>For <code>AntennaUplinkConfig</code>, valid values are between 10 kHz to 54 MHz.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"units\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-frequency-bandwidth-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: FrequencyBandwidth
---
