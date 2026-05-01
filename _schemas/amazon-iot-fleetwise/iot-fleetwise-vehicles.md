---
description: vehicles schema
layout: schema
name: vehicles
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-vehicles-schema.json
slug: iot-fleetwise-vehicles
source_filename: iot-fleetwise-vehicles-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-vehicles-schema.json\",\n  \"title\": \"vehicles\",\n  \"description\": \"vehicles schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[a-zA-Z\\\\d\\\\-_:]+\",\n    \"minLength\": 1,\n    \"maxLength\": 100\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-vehicles-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: vehicles
---
