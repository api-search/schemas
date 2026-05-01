---
description: fleets schema
layout: schema
name: fleets
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-fleets-schema.json
slug: iot-fleetwise-fleets
source_filename: iot-fleetwise-fleets-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-fleets-schema.json\",\n  \"title\": \"fleets\",\n  \"description\": \"fleets schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z0-9:_-]+\",\n    \"minLength\": 1,\n    \"maxLength\": 100\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-fleets-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: fleets
---
