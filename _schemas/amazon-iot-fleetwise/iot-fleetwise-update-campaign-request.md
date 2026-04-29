---
description: UpdateCampaignRequest schema
layout: schema
name: UpdateCampaignRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: dataExtraDimensions
  type: object
- description: ''
  name: action
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-update-campaign-request-schema.json
slug: iot-fleetwise-update-campaign-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-campaign-request-schema.json\",\n  \"title\": \"UpdateCampaignRequest\",\n  \"description\": \"UpdateCampaignRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/campaignName\"\n        },\n        {\n          \"description\": \" The name of the campaign to update. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"The description of the campaign.\"\n        }\n      ]\n    },\n    \"dataExtraDimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataExtraDimensionNodePathList\"\n        },\n   \
  \     {\n          \"description\": \"<p> A list of vehicle attributes to associate with a signal. </p> <p>Default: An empty array</p>\"\n        }\n      ]\n    },\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateCampaignAction\"\n        },\n        {\n          \"description\": \"<p> Specifies how to update a campaign. The action can be one of the following:</p> <ul> <li> <p> <code>APPROVE</code> - To approve delivering a data collection scheme to vehicles. </p> </li> <li> <p> <code>SUSPEND</code> - To suspend collecting signal data. The campaign is deleted from vehicles and all vehicles in the suspended campaign will stop sending data.</p> </li> <li> <p> <code>RESUME</code> - To reactivate the <code>SUSPEND</code> campaign. The campaign is redeployed to all vehicles and the vehicles will resume sending data.</p> </li> <li> <p> <code>UPDATE</code> - To update a campaign. </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"name\",\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-update-campaign-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: UpdateCampaignRequest
---
