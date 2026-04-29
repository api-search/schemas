---
description: Information about the uplink <code>Config</code> of an antenna.
layout: schema
name: AntennaUplinkConfig
properties_list:
- description: ''
  name: spectrumConfig
  type: object
- description: ''
  name: targetEirp
  type: object
- description: ''
  name: transmitDisabled
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-antenna-uplink-config-schema.json
slug: ground-station-antenna-uplink-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-antenna-uplink-config-schema.json\",\n  \"title\": \"AntennaUplinkConfig\",\n  \"description\": \"Information about the uplink <code>Config</code> of an antenna.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spectrumConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UplinkSpectrumConfig\"\n        },\n        {\n          \"description\": \"Information about the uplink spectral <code>Config</code>.\"\n        }\n      ]\n    },\n    \"targetEirp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eirp\"\n        },\n        {\n          \"description\": \"EIRP of the target.\"\n        }\n      ]\n    },\n    \"transmitDisabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\
  \n        },\n        {\n          \"description\": \"Whether or not uplink transmit is disabled.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spectrumConfig\",\n    \"targetEirp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-antenna-uplink-config-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: AntennaUplinkConfig
---
