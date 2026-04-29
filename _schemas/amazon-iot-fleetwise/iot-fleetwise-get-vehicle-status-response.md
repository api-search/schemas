---
description: GetVehicleStatusResponse schema
layout: schema
name: GetVehicleStatusResponse
properties_list:
- description: ''
  name: campaigns
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-get-vehicle-status-response-schema.json
slug: iot-fleetwise-get-vehicle-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-vehicle-status-response-schema.json\",\n  \"title\": \"GetVehicleStatusResponse\",\n  \"description\": \"GetVehicleStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaigns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VehicleStatusList\"\n        },\n        {\n          \"description\": \" Lists information about the state of the vehicle with deployed campaigns. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \" The token to retrieve the next set of results, or <code>null</code> if there are no more results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-vehicle-status-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: GetVehicleStatusResponse
---
