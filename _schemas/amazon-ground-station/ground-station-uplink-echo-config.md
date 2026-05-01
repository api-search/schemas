---
description: <p>Information about an uplink echo <code>Config</code>.</p> <p>Parameters from the <code>AntennaUplinkConfig</code>, corresponding to the specified <code>AntennaUplinkConfigArn</code>, are used when this <code>UplinkEchoConfig</code> is used in a contact.</p>
layout: schema
name: UplinkEchoConfig
properties_list:
- description: ''
  name: antennaUplinkConfigArn
  type: object
- description: ''
  name: enabled
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-uplink-echo-config-schema.json
slug: ground-station-uplink-echo-config
source_filename: ground-station-uplink-echo-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-uplink-echo-config-schema.json\",\n  \"title\": \"UplinkEchoConfig\",\n  \"description\": \"<p>Information about an uplink echo <code>Config</code>.</p> <p>Parameters from the <code>AntennaUplinkConfig</code>, corresponding to the specified <code>AntennaUplinkConfigArn</code>, are used when this <code>UplinkEchoConfig</code> is used in a contact.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"antennaUplinkConfigArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigArn\"\n        },\n        {\n          \"description\": \"ARN of an uplink <code>Config</code>.\"\n        }\n      ]\n    },\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\"\
  : \"Whether or not an uplink <code>Config</code> is enabled.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"antennaUplinkConfigArn\",\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-uplink-echo-config-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: UplinkEchoConfig
---
