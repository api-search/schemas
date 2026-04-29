---
description: DeleteFleetRequest schema
layout: schema
name: DeleteFleetRequest
properties_list:
- description: ''
  name: fleetId
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-delete-fleet-request-schema.json
slug: iot-fleetwise-delete-fleet-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-fleet-request-schema.json\",\n  \"title\": \"DeleteFleetRequest\",\n  \"description\": \"DeleteFleetRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/fleetId\"\n        },\n        {\n          \"description\": \" The ID of the fleet to delete. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-fleet-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: DeleteFleetRequest
---
