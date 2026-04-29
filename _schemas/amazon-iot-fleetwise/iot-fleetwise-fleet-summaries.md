---
description: fleetSummaries schema
layout: schema
name: fleetSummaries
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-fleet-summaries-schema.json
slug: iot-fleetwise-fleet-summaries
source_filename: iot-fleetwise-fleet-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-fleet-summaries-schema.json\",\n  \"title\": \"fleetSummaries\",\n  \"description\": \"fleetSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"id\",\n      \"arn\",\n      \"signalCatalogArn\",\n      \"creationTime\"\n    ],\n    \"properties\": {\n      \"id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/fleetId\"\n          },\n          {\n            \"description\": \"The unique ID of the fleet.\"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of the fleet.\"\n          }\n        ]\n      },\n \
  \     \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/description\"\n          },\n          {\n            \"description\": \"A brief description of the fleet.\"\n          }\n        ]\n      },\n      \"signalCatalogArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of the signal catalog associated with the fleet.\"\n          }\n        ]\n      },\n      \"creationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/timestamp\"\n          },\n          {\n            \"description\": \"The time the fleet was created, in seconds since epoch (January 1, 1970 at midnight UTC time).\"\n          }\n        ]\n      },\n      \"lastModificationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/timestamp\"\n          },\n          {\n            \"\
  description\": \"The time the fleet was last updated in seconds since epoch (January 1, 1970 at midnight UTC time).\"\n          }\n        ]\n      }\n    },\n    \"description\": \"<p>Information about a fleet.</p> <p>You can use the API operation to return this information about multiple fleets.</p>\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-fleet-summaries-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: fleetSummaries
---
