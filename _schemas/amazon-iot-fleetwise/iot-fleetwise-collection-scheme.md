---
description: Specifies what data to collect and how often or when to collect it.
layout: schema
name: CollectionScheme
properties_list:
- description: ''
  name: timeBasedCollectionScheme
  type: object
- description: ''
  name: conditionBasedCollectionScheme
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-collection-scheme-schema.json
slug: iot-fleetwise-collection-scheme
source_filename: iot-fleetwise-collection-scheme-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-collection-scheme-schema.json\",\n  \"title\": \"CollectionScheme\",\n  \"description\": \"Specifies what data to collect and how often or when to collect it.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timeBasedCollectionScheme\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeBasedCollectionScheme\"\n        },\n        {\n          \"description\": \"Information about a collection scheme that uses a time period to decide how often to collect data.\"\n        }\n      ]\n    },\n    \"conditionBasedCollectionScheme\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConditionBasedCollectionScheme\"\n        },\n        {\n          \"description\": \"Information about a collection scheme that uses a simple logical\
  \ expression to recognize what data to collect.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-collection-scheme-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CollectionScheme
---
