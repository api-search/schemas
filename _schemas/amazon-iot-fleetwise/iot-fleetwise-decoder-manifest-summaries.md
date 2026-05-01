---
description: decoderManifestSummaries schema
layout: schema
name: decoderManifestSummaries
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-decoder-manifest-summaries-schema.json
slug: iot-fleetwise-decoder-manifest-summaries
source_filename: iot-fleetwise-decoder-manifest-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-decoder-manifest-summaries-schema.json\",\n  \"title\": \"decoderManifestSummaries\",\n  \"description\": \"decoderManifestSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"creationTime\",\n      \"lastModificationTime\"\n    ],\n    \"properties\": {\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/string\"\n          },\n          {\n            \"description\": \"The name of the decoder manifest.\"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of a vehicle model (model manifest) associated with the decoder manifest.\
  \ \"\n          }\n        ]\n      },\n      \"modelManifestArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of a vehicle model (model manifest) associated with the decoder manifest.\"\n          }\n        ]\n      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/description\"\n          },\n          {\n            \"description\": \"A brief description of the decoder manifest.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ManifestStatus\"\n          },\n          {\n            \"description\": \"The state of the decoder manifest. If the status is <code>ACTIVE</code>, the decoder manifest can't be edited. If the status is marked <code>DRAFT</code>, you can edit the decoder manifest.\"\n          }\n        ]\n      },\n\
  \      \"creationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/timestamp\"\n          },\n          {\n            \"description\": \"The time the decoder manifest was created in seconds since epoch (January 1, 1970 at midnight UTC time).\"\n          }\n        ]\n      },\n      \"lastModificationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/timestamp\"\n          },\n          {\n            \"description\": \"The time the decoder manifest was last updated in seconds since epoch (January 1, 1970 at midnight UTC time).\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about a created decoder manifest. You can use the API operation to return this information about multiple decoder manifests.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-decoder-manifest-summaries-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: decoderManifestSummaries
---
