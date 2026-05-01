---
description: <p>Information about a vehicle.</p> <p>To return this information about vehicles in your account, you can use the API operation.</p>
layout: schema
name: VehicleSummary
properties_list:
- description: ''
  name: vehicleName
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: modelManifestArn
  type: object
- description: ''
  name: decoderManifestArn
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: lastModificationTime
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-vehicle-summary-schema.json
slug: iot-fleetwise-vehicle-summary
source_filename: iot-fleetwise-vehicle-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-vehicle-summary-schema.json\",\n  \"title\": \"VehicleSummary\",\n  \"description\": \"<p>Information about a vehicle.</p> <p>To return this information about vehicles in your account, you can use the API operation.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicleName\"\n        },\n        {\n          \"description\": \"The unique ID of the vehicle.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the vehicle.\"\n        }\n      ]\n    },\n    \"modelManifestArn\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The ARN of a vehicle model (model manifest) associated with the vehicle.\"\n        }\n      ]\n    },\n    \"decoderManifestArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The ARN of a decoder manifest associated with the vehicle.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The time the vehicle was created in seconds since epoch (January 1, 1970 at midnight UTC time).\"\n        }\n      ]\n    },\n    \"lastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The time the vehicle was last updated in seconds since epoch (January 1, 1970 at midnight\
  \ UTC time). \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicleName\",\n    \"arn\",\n    \"modelManifestArn\",\n    \"decoderManifestArn\",\n    \"creationTime\",\n    \"lastModificationTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-vehicle-summary-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: VehicleSummary
---
