---
description: ListFleetsResponse schema
layout: schema
name: ListFleetsResponse
properties_list:
- description: ''
  name: fleetSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-list-fleets-response-schema.json
slug: iot-fleetwise-list-fleets-response
source_filename: iot-fleetwise-list-fleets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-fleets-response-schema.json\",\n  \"title\": \"ListFleetsResponse\",\n  \"description\": \"ListFleetsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleetSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/fleetSummaries\"\n        },\n        {\n          \"description\": \" A list of information for each fleet. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \" The token to retrieve the next set of results, or <code>null</code> if there are no more results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-fleets-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ListFleetsResponse
---
