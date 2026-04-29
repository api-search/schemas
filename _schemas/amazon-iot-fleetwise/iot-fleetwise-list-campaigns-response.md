---
description: ListCampaignsResponse schema
layout: schema
name: ListCampaignsResponse
properties_list:
- description: ''
  name: campaignSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-list-campaigns-response-schema.json
slug: iot-fleetwise-list-campaigns-response
source_filename: iot-fleetwise-list-campaigns-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-campaigns-response-schema.json\",\n  \"title\": \"ListCampaignsResponse\",\n  \"description\": \"ListCampaignsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/campaignSummaries\"\n        },\n        {\n          \"description\": \" A summary of information about each campaign. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \" The token to retrieve the next set of results, or <code>null</code> if there are no more results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-campaigns-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ListCampaignsResponse
---
