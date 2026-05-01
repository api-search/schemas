---
description: UpdateCampaignResponse schema
layout: schema
name: UpdateCampaignResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-campaign-response-schema.json
slug: iot-fleetwise-update-campaign-response
source_filename: iot-fleetwise-update-campaign-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-campaign-response-schema.json\",\n  \"title\": \"UpdateCampaignResponse\",\n  \"description\": \"UpdateCampaignResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the campaign. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/campaignName\"\n        },\n        {\n          \"description\": \"The name of the updated campaign.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignStatus\"\n        },\n        {\n          \"description\"\
  : \"<p>The state of a campaign. The status can be one of:</p> <ul> <li> <p> <code>CREATING</code> - Amazon Web Services IoT FleetWise is processing your request to create the campaign. </p> </li> <li> <p> <code>WAITING_FOR_APPROVAL</code> - After a campaign is created, it enters the <code>WAITING_FOR_APPROVAL</code> state. To allow Amazon Web Services IoT FleetWise to deploy the campaign to the target vehicle or fleet, use the API operation to approve the campaign. </p> </li> <li> <p> <code>RUNNING</code> - The campaign is active. </p> </li> <li> <p> <code>SUSPENDED</code> - The campaign is suspended. To resume the campaign, use the API operation. </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-campaign-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: UpdateCampaignResponse
---
