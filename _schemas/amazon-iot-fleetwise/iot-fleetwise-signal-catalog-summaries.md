---
description: signalCatalogSummaries schema
layout: schema
name: signalCatalogSummaries
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-signal-catalog-summaries-schema.json
slug: iot-fleetwise-signal-catalog-summaries
source_filename: iot-fleetwise-signal-catalog-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-signal-catalog-summaries-schema.json\",\n  \"title\": \"signalCatalogSummaries\",\n  \"description\": \"signalCatalogSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/string\"\n          },\n          {\n            \"description\": \"The name of the signal catalog.\"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of the signal catalog.\"\n          }\n        ]\n      },\n      \"creationTime\": {\n        \"allOf\": [\n          {\n            \"\
  $ref\": \"#/components/schemas/timestamp\"\n          },\n          {\n            \"description\": \"The time the signal catalog was created in seconds since epoch (January 1, 1970 at midnight UTC time). \"\n          }\n        ]\n      },\n      \"lastModificationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/timestamp\"\n          },\n          {\n            \"description\": \"The time the signal catalog was last updated in seconds since epoch (January 1, 1970 at midnight UTC time). \"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about a collection of standardized signals, which can be attributes, branches, sensors, or actuators.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-signal-catalog-summaries-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: signalCatalogSummaries
---
