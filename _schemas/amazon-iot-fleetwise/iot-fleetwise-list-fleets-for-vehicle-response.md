---
description: ListFleetsForVehicleResponse schema
layout: schema
name: ListFleetsForVehicleResponse
properties_list:
- description: ''
  name: fleets
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-list-fleets-for-vehicle-response-schema.json
slug: iot-fleetwise-list-fleets-for-vehicle-response
source_filename: iot-fleetwise-list-fleets-for-vehicle-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-fleets-for-vehicle-response-schema.json\",\n  \"title\": \"ListFleetsForVehicleResponse\",\n  \"description\": \"ListFleetsForVehicleResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/fleets\"\n        },\n        {\n          \"description\": \" A list of fleet IDs that the vehicle is associated with. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \" The token to retrieve the next set of results, or <code>null</code> if there are no more results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-fleets-for-vehicle-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ListFleetsForVehicleResponse
---
