---
description: ListVehiclesInFleetResponse schema
layout: schema
name: ListVehiclesInFleetResponse
properties_list:
- description: ''
  name: vehicles
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-list-vehicles-in-fleet-response-schema.json
slug: iot-fleetwise-list-vehicles-in-fleet-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-vehicles-in-fleet-response-schema.json\",\n  \"title\": \"ListVehiclesInFleetResponse\",\n  \"description\": \"ListVehiclesInFleetResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vehicles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/vehicles\"\n        },\n        {\n          \"description\": \" A list of vehicles associated with the fleet. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \" The token to retrieve the next set of results, or <code>null</code> if there are no more results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-vehicles-in-fleet-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ListVehiclesInFleetResponse
---
