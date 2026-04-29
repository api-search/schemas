---
description: Information about the vehicle to update.
layout: schema
name: UpdateVehicleRequestItem
properties_list:
- description: ''
  name: vehicleName
  type: object
- description: ''
  name: modelManifestArn
  type: object
- description: ''
  name: decoderManifestArn
  type: object
- description: ''
  name: attributes
  type: object
- description: ''
  name: attributeUpdateMode
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-vehicle-request-item-schema.json
slug: iot-fleetwise-update-vehicle-request-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-vehicle-request-item-schema.json\",\n  \"title\": \"UpdateVehicleRequestItem\",\n  \"description\": \"Information about the vehicle to update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicleName\"\n        },\n        {\n          \"description\": \"The unique ID of the vehicle to update.\"\n        }\n      ]\n    },\n    \"modelManifestArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The ARN of the vehicle model (model manifest) associated with the vehicle to update.\"\n        }\n      ]\n    },\n    \"decoderManifestArn\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The ARN of the signal decoder manifest associated with the vehicle to update.\"\n        }\n      ]\n    },\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/attributesMap\"\n        },\n        {\n          \"description\": \"<p>Static information about a vehicle in a key-value pair. For example:</p> <p> <code>\\\"engineType\\\"</code> : <code>\\\"1.3 L R2\\\"</code> </p>\"\n        }\n      ]\n    },\n    \"attributeUpdateMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateMode\"\n        },\n        {\n          \"description\": \"<p>The method the specified attributes will update the existing attributes on the vehicle. Use<code>Overwite</code> to replace the vehicle attributes with the specified attributes. Or use <code>Merge</code> to combine all attributes.</p> <p>This is required if attributes are present in the\
  \ input.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-vehicle-request-item-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: UpdateVehicleRequestItem
---
