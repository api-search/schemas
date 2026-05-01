---
description: GetFleetRequest schema
layout: schema
name: GetFleetRequest
properties_list:
- description: ''
  name: fleetId
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-get-fleet-request-schema.json
slug: iot-fleetwise-get-fleet-request
source_filename: iot-fleetwise-get-fleet-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-fleet-request-schema.json\",\n  \"title\": \"GetFleetRequest\",\n  \"description\": \"GetFleetRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/fleetId\"\n        },\n        {\n          \"description\": \" The ID of the fleet to retrieve information about. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-fleet-request-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: GetFleetRequest
---
