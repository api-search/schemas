---
description: campaignSummaries schema
layout: schema
name: campaignSummaries
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-campaign-summaries-schema.json
slug: iot-fleetwise-campaign-summaries
source_filename: iot-fleetwise-campaign-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-campaign-summaries-schema.json\",\n  \"title\": \"campaignSummaries\",\n  \"description\": \"campaignSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"creationTime\",\n      \"lastModificationTime\"\n    ],\n    \"properties\": {\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The Amazon Resource Name (ARN) of a campaign.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/campaignName\"\n          },\n          {\n            \"description\": \"The name of a campaign.\"\n          }\n        ]\n      },\n      \"description\"\
  : {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/description\"\n          },\n          {\n            \"description\": \"The description of the campaign.\"\n          }\n        ]\n      },\n      \"signalCatalogArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of the signal catalog associated with the campaign.\"\n          }\n        ]\n      },\n      \"targetArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/arn\"\n          },\n          {\n            \"description\": \"The ARN of a vehicle or fleet to which the campaign is deployed.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CampaignStatus\"\n          },\n          {\n            \"description\": \"<p>The state of a campaign. The status can be one of\
  \ the following:</p> <ul> <li> <p> <code>CREATING</code> - Amazon Web Services IoT FleetWise is processing your request to create the campaign.</p> </li> <li> <p> <code>WAITING_FOR_APPROVAL</code> - After a campaign is created, it enters the <code>WAITING_FOR_APPROVAL</code> state. To allow Amazon Web Services IoT FleetWise to deploy the campaign to the target vehicle or fleet, use the API operation to approve the campaign. </p> </li> <li> <p> <code>RUNNING</code> - The campaign is active. </p> </li> <li> <p> <code>SUSPENDED</code> - The campaign is suspended. To resume the campaign, use the API operation. </p> </li> </ul>\"\n          }\n        ]\n      },\n      \"creationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/timestamp\"\n          },\n          {\n            \"description\": \"The time the campaign was created.\"\n          }\n        ]\n      },\n      \"lastModificationTime\": {\n        \"allOf\": [\n          {\n           \
  \ \"$ref\": \"#/components/schemas/timestamp\"\n          },\n          {\n            \"description\": \"The last time the campaign was modified.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"<p>Information about a campaign. </p> <p>You can use the API operation to return this information about multiple created campaigns.</p>\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-campaign-summaries-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: campaignSummaries
---
