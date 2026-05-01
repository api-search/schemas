---
description: DeleteCampaignResponse schema
layout: schema
name: DeleteCampaignResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-delete-campaign-response-schema.json
slug: iot-fleetwise-delete-campaign-response
source_filename: iot-fleetwise-delete-campaign-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-campaign-response-schema.json\",\n  \"title\": \"DeleteCampaignResponse\",\n  \"description\": \"DeleteCampaignResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/campaignName\"\n        },\n        {\n          \"description\": \"The name of the deleted campaign.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"<p> The Amazon Resource Name (ARN) of the deleted campaign.</p> <note> <p>The ARN isn\\u2019t returned if a campaign doesn\\u2019t exist.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-delete-campaign-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: DeleteCampaignResponse
---
