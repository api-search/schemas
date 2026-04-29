---
description: Information about a collection scheme that uses a time period to decide how often to collect data.
layout: schema
name: TimeBasedCollectionScheme
properties_list:
- description: ''
  name: periodMs
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-time-based-collection-scheme-schema.json
slug: iot-fleetwise-time-based-collection-scheme
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-time-based-collection-scheme-schema.json\",\n  \"title\": \"TimeBasedCollectionScheme\",\n  \"description\": \"Information about a collection scheme that uses a time period to decide how often to collect data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"periodMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/collectionPeriodMs\"\n        },\n        {\n          \"description\": \"The time period (in milliseconds) to decide how often to collect data. For example, if the time period is <code>60000</code>, the Edge Agent software collects data once every minute.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"periodMs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-time-based-collection-scheme-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: TimeBasedCollectionScheme
---
