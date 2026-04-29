---
description: UpdateFleetRequest schema
layout: schema
name: UpdateFleetRequest
properties_list:
- description: ''
  name: fleetId
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-fleet-request-schema.json
slug: iot-fleetwise-update-fleet-request
source_filename: iot-fleetwise-update-fleet-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-fleet-request-schema.json\",\n  \"title\": \"UpdateFleetRequest\",\n  \"description\": \"UpdateFleetRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/fleetId\"\n        },\n        {\n          \"description\": \" The ID of the fleet to update. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \" An updated description of the fleet. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-fleet-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: UpdateFleetRequest
---
