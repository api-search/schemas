---
description: UpdateDecoderManifestRequest schema
layout: schema
name: UpdateDecoderManifestRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: signalDecodersToAdd
  type: object
- description: ''
  name: signalDecodersToUpdate
  type: object
- description: ''
  name: signalDecodersToRemove
  type: object
- description: ''
  name: networkInterfacesToAdd
  type: object
- description: ''
  name: networkInterfacesToUpdate
  type: object
- description: ''
  name: networkInterfacesToRemove
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-decoder-manifest-request-schema.json
slug: iot-fleetwise-update-decoder-manifest-request
source_filename: iot-fleetwise-update-decoder-manifest-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-decoder-manifest-request-schema.json\",\n  \"title\": \"UpdateDecoderManifestRequest\",\n  \"description\": \"UpdateDecoderManifestRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/resourceName\"\n        },\n        {\n          \"description\": \" The name of the decoder manifest to update.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \" A brief description of the decoder manifest to update. \"\n        }\n      ]\n    },\n    \"signalDecodersToAdd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalDecoders\"\
  \n        },\n        {\n          \"description\": \" A list of information about decoding additional signals to add to the decoder manifest. \"\n        }\n      ]\n    },\n    \"signalDecodersToUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalDecoders\"\n        },\n        {\n          \"description\": \" A list of updated information about decoding signals to update in the decoder manifest. \"\n        }\n      ]\n    },\n    \"signalDecodersToRemove\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Fqns\"\n        },\n        {\n          \"description\": \" A list of signal decoders to remove from the decoder manifest. \"\n        }\n      ]\n    },\n    \"networkInterfacesToAdd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaces\"\n        },\n        {\n          \"description\": \" A list of information about the network interfaces to add to the decoder manifest.\
  \ \"\n        }\n      ]\n    },\n    \"networkInterfacesToUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaces\"\n        },\n        {\n          \"description\": \" A list of information about the network interfaces to update in the decoder manifest. \"\n        }\n      ]\n    },\n    \"networkInterfacesToRemove\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterfaceIds\"\n        },\n        {\n          \"description\": \" A list of network interfaces to remove from the decoder manifest.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestStatus\"\n        },\n        {\n          \"description\": \" The state of the decoder manifest. If the status is <code>ACTIVE</code>, the decoder manifest can't be edited. If the status is <code>DRAFT</code>, you can edit the decoder manifest. \"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-decoder-manifest-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: UpdateDecoderManifestRequest
---
