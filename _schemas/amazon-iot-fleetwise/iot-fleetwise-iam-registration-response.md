---
description: Information about registering an Identity and Access Management (IAM) resource so Amazon Web Services IoT FleetWise edge agent software can transfer your vehicle data to Amazon Timestream.
layout: schema
name: IamRegistrationResponse
properties_list:
- description: ''
  name: roleArn
  type: object
- description: ''
  name: registrationStatus
  type: object
- description: ''
  name: errorMessage
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-iam-registration-response-schema.json
slug: iot-fleetwise-iam-registration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-iam-registration-response-schema.json\",\n  \"title\": \"IamRegistrationResponse\",\n  \"description\": \"Information about registering an Identity and Access Management (IAM) resource so Amazon Web Services IoT FleetWise edge agent software can transfer your vehicle data to Amazon Timestream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role to register.\"\n        }\n      ]\n    },\n    \"registrationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \"The status of registering\
  \ your IAM resource. The status can be one of <code>REGISTRATION_SUCCESS</code>, <code>REGISTRATION_PENDING</code>, <code>REGISTRATION_FAILURE</code>.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/errorMessage\"\n        },\n        {\n          \"description\": \"A message associated with a registration error.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"roleArn\",\n    \"registrationStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-iam-registration-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: IamRegistrationResponse
---
