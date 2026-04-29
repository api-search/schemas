---
description: Information about a created decoder manifest. You can use the API operation to return this information about multiple decoder manifests.
layout: schema
name: DecoderManifestSummary
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: modelManifestArn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: lastModificationTime
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-decoder-manifest-summary-schema.json
slug: iot-fleetwise-decoder-manifest-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-decoder-manifest-summary-schema.json\",\n  \"title\": \"DecoderManifestSummary\",\n  \"description\": \"Information about a created decoder manifest. You can use the API operation to return this information about multiple decoder manifests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The name of the decoder manifest.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The ARN of a vehicle model (model manifest) associated with the decoder manifest. \"\n        }\n      ]\n    },\n    \"modelManifestArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The ARN of a vehicle model (model manifest) associated with the decoder manifest.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"A brief description of the decoder manifest.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestStatus\"\n        },\n        {\n          \"description\": \"The state of the decoder manifest. If the status is <code>ACTIVE</code>, the decoder manifest can't be edited. If the status is marked <code>DRAFT</code>, you can edit the decoder manifest.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n\
  \        {\n          \"description\": \"The time the decoder manifest was created in seconds since epoch (January 1, 1970 at midnight UTC time).\"\n        }\n      ]\n    },\n    \"lastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The time the decoder manifest was last updated in seconds since epoch (January 1, 1970 at midnight UTC time).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"creationTime\",\n    \"lastModificationTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-decoder-manifest-summary-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: DecoderManifestSummary
---
