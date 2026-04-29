---
description: VehicleStatusList schema
layout: schema
name: VehicleStatusList
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-vehicle-status-list-schema.json
slug: iot-fleetwise-vehicle-status-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-vehicle-status-list-schema.json\",\n  \"title\": \"VehicleStatusList\",\n  \"description\": \"VehicleStatusList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"campaignName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/string\"\n          },\n          {\n            \"description\": \"The name of a campaign.\"\n          }\n        ]\n      },\n      \"vehicleName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/vehicleName\"\n          },\n          {\n            \"description\": \"The unique ID of the vehicle.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/VehicleState\"\
  \n          },\n          {\n            \"description\": \"<p>The state of a vehicle, which can be one of the following:</p> <ul> <li> <p> <code>CREATED</code> - Amazon Web Services IoT FleetWise sucessfully created the vehicle. </p> </li> <li> <p> <code>READY</code> - The vehicle is ready to receive a campaign deployment. </p> </li> <li> <p> <code>HEALTHY</code> - A campaign deployment was delivered to the vehicle. </p> </li> <li> <p> <code>SUSPENDED</code> - A campaign associated with the vehicle was suspended and data collection was paused. </p> </li> <li> <p> <code>DELETING</code> - Amazon Web Services IoT FleetWise is removing a campaign from the vehicle. </p> </li> </ul>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about the state of a vehicle and how it relates to the status of a campaign.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-vehicle-status-list-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: VehicleStatusList
---
