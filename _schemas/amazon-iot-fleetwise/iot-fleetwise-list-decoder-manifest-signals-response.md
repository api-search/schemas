---
description: ListDecoderManifestSignalsResponse schema
layout: schema
name: ListDecoderManifestSignalsResponse
properties_list:
- description: ''
  name: signalDecoders
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-list-decoder-manifest-signals-response-schema.json
slug: iot-fleetwise-list-decoder-manifest-signals-response
source_filename: iot-fleetwise-list-decoder-manifest-signals-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-decoder-manifest-signals-response-schema.json\",\n  \"title\": \"ListDecoderManifestSignalsResponse\",\n  \"description\": \"ListDecoderManifestSignalsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"signalDecoders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalDecoders\"\n        },\n        {\n          \"description\": \" Information about a list of signals to decode. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \" The token to retrieve the next set of results, or <code>null</code> if there are no more results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-decoder-manifest-signals-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ListDecoderManifestSignalsResponse
---
