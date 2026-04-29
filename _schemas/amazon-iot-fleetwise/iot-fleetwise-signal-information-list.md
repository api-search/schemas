---
description: SignalInformationList schema
layout: schema
name: SignalInformationList
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-signal-information-list-schema.json
slug: iot-fleetwise-signal-information-list
source_filename: iot-fleetwise-signal-information-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-signal-information-list-schema.json\",\n  \"title\": \"SignalInformationList\",\n  \"description\": \"SignalInformationList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"name\"\n    ],\n    \"properties\": {\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/wildcardSignalName\"\n          },\n          {\n            \"description\": \"The name of the signal.\"\n          }\n        ]\n      },\n      \"maxSampleCount\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/maxSampleCount\"\n          },\n          {\n            \"description\": \"The maximum number of samples to collect.\"\n          }\n        ]\n      },\n      \"minimumSamplingIntervalMs\"\
  : {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/uint32\"\n          },\n          {\n            \"description\": \"<p>The minimum duration of time (in milliseconds) between two triggering events to collect data.</p> <note> <p>If a signal changes often, you might want to collect data at a slower rate.</p> </note>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about a signal.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-signal-information-list-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: SignalInformationList
---
