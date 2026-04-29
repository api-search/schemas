---
description: <p>Object containing the parameters of a <code>Config</code>.</p> <p>See the subtype definitions for what each type of <code>Config</code> contains.</p>
layout: schema
name: ConfigTypeData
properties_list:
- description: ''
  name: antennaDownlinkConfig
  type: object
- description: ''
  name: antennaDownlinkDemodDecodeConfig
  type: object
- description: ''
  name: antennaUplinkConfig
  type: object
- description: ''
  name: dataflowEndpointConfig
  type: object
- description: ''
  name: s3RecordingConfig
  type: object
- description: ''
  name: trackingConfig
  type: object
- description: ''
  name: uplinkEchoConfig
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-config-type-data-schema.json
slug: ground-station-config-type-data
source_filename: ground-station-config-type-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-config-type-data-schema.json\",\n  \"title\": \"ConfigTypeData\",\n  \"description\": \"<p>Object containing the parameters of a <code>Config</code>.</p> <p>See the subtype definitions for what each type of <code>Config</code> contains.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"antennaDownlinkConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AntennaDownlinkConfig\"\n        },\n        {\n          \"description\": \"Information about how AWS Ground Station should configure an antenna for downlink during a contact.\"\n        }\n      ]\n    },\n    \"antennaDownlinkDemodDecodeConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AntennaDownlinkDemodDecodeConfig\"\n        },\n        {\n      \
  \    \"description\": \"Information about how AWS Ground Station should con\\ufb01gure an antenna for downlink demod decode during a contact.\"\n        }\n      ]\n    },\n    \"antennaUplinkConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AntennaUplinkConfig\"\n        },\n        {\n          \"description\": \"Information about how AWS Ground Station should con\\ufb01gure an antenna for uplink during a contact.\"\n        }\n      ]\n    },\n    \"dataflowEndpointConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEndpointConfig\"\n        },\n        {\n          \"description\": \"Information about the dataflow endpoint <code>Config</code>.\"\n        }\n      ]\n    },\n    \"s3RecordingConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3RecordingConfig\"\n        },\n        {\n          \"description\": \"Information about an S3 recording <code>Config</code>.\"\
  \n        }\n      ]\n    },\n    \"trackingConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrackingConfig\"\n        },\n        {\n          \"description\": \"Object that determines whether tracking should be used during a contact executed with this <code>Config</code> in the mission profile. \"\n        }\n      ]\n    },\n    \"uplinkEchoConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UplinkEchoConfig\"\n        },\n        {\n          \"description\": \"<p>Information about an uplink echo <code>Config</code>.</p> <p>Parameters from the <code>AntennaUplinkConfig</code>, corresponding to the specified <code>AntennaUplinkConfigArn</code>, are used when this <code>UplinkEchoConfig</code> is used in a contact.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-config-type-data-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ConfigTypeData
---
