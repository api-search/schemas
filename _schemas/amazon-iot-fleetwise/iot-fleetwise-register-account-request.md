---
description: RegisterAccountRequest schema
layout: schema
name: RegisterAccountRequest
properties_list:
- description: ''
  name: timestreamResources
  type: object
- description: ''
  name: iamResources
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-register-account-request-schema.json
slug: iot-fleetwise-register-account-request
source_filename: iot-fleetwise-register-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-register-account-request-schema.json\",\n  \"title\": \"RegisterAccountRequest\",\n  \"description\": \"RegisterAccountRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestreamResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamResources\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"Amazon Timestream metadata is now passed in the CreateCampaign API.\"\n        }\n      ]\n    },\n    \"iamResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamResources\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"The IAM resource that allows Amazon Web Services IoT FleetWise to send data to Amazon Timestream.iamResources\
  \ is no longer used or needed as input\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-register-account-request-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: RegisterAccountRequest
---
