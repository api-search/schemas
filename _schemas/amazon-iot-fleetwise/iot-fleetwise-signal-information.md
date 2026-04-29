---
description: Information about a signal.
layout: schema
name: SignalInformation
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: maxSampleCount
  type: object
- description: ''
  name: minimumSamplingIntervalMs
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-signal-information-schema.json
slug: iot-fleetwise-signal-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-signal-information-schema.json\",\n  \"title\": \"SignalInformation\",\n  \"description\": \"Information about a signal.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/wildcardSignalName\"\n        },\n        {\n          \"description\": \"The name of the signal.\"\n        }\n      ]\n    },\n    \"maxSampleCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/maxSampleCount\"\n        },\n        {\n          \"description\": \"The maximum number of samples to collect.\"\n        }\n      ]\n    },\n    \"minimumSamplingIntervalMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/uint32\"\n        },\n        {\n          \"description\"\
  : \"<p>The minimum duration of time (in milliseconds) between two triggering events to collect data.</p> <note> <p>If a signal changes often, you might want to collect data at a slower rate.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-signal-information-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: SignalInformation
---
