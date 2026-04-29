---
description: CreateVehicleRequest schema
layout: schema
name: CreateVehicleRequest
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
  name: associationBehavior
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-vehicle-request-schema.json
slug: iot-fleetwise-create-vehicle-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-vehicle-request-schema.json\",\n  \"title\": \"CreateVehicleRequest\",\n  \"description\": \"CreateVehicleRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicleName\"\n        },\n        {\n          \"description\": \" The unique ID of the vehicle to create. \"\n        }\n      ]\n    },\n    \"modelManifestArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name ARN of a vehicle model. \"\n        }\n      ]\n    },\n    \"decoderManifestArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n\
  \          \"description\": \" The ARN of a decoder manifest. \"\n        }\n      ]\n    },\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/attributesMap\"\n        },\n        {\n          \"description\": \"<p>Static information about a vehicle in a key-value pair. For example: <code>\\\"engineType\\\"</code> : <code>\\\"1.3 L R2\\\"</code> </p> <p>A campaign must include the keys (attribute names) in <code>dataExtraDimensions</code> for them to display in Amazon Timestream.</p>\"\n        }\n      ]\n    },\n    \"associationBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VehicleAssociationBehavior\"\n        },\n        {\n          \"description\": \"<p> An option to create a new Amazon Web Services IoT thing when creating a vehicle, or to validate an existing Amazon Web Services IoT thing as a vehicle. </p> <p>Default: <code/> </p>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Metadata that can be used to manage the vehicle.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"vehicleName\",\n    \"modelManifestArn\",\n    \"decoderManifestArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-vehicle-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CreateVehicleRequest
---
