---
description: RegisterAccountResponse schema
layout: schema
name: RegisterAccountResponse
properties_list:
- description: ''
  name: registerAccountStatus
  type: object
- description: The registered Amazon Timestream resources that Amazon Web Services IoT FleetWise edge agent software can transfer your vehicle data to.
  name: timestreamResources
  type: object
- description: ''
  name: iamResources
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: lastModificationTime
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-register-account-response-schema.json
slug: iot-fleetwise-register-account-response
source_filename: iot-fleetwise-register-account-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-register-account-response-schema.json\",\n  \"title\": \"RegisterAccountResponse\",\n  \"description\": \"RegisterAccountResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"registerAccountStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \" The status of registering your Amazon Web Services account, IAM role, and Timestream resources. \"\n        }\n      ]\n    },\n    \"timestreamResources\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"timestreamDatabaseName\",\n        \"timestreamTableName\"\n      ],\n      \"properties\": {\n        \"timestreamDatabaseName\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/TimestreamDatabaseName\"\
  \n            },\n            {\n              \"description\": \"The name of the registered Amazon Timestream database.\"\n            }\n          ]\n        },\n        \"timestreamTableName\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/TimestreamTableName\"\n            },\n            {\n              \"description\": \"The name of the registered Amazon Timestream database table.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"The registered Amazon Timestream resources that Amazon Web Services IoT FleetWise edge agent software can transfer your vehicle data to.\"\n    },\n    \"iamResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamResources\"\n        },\n        {\n          \"description\": \" The registered IAM resource that allows Amazon Web Services IoT FleetWise to send data to Amazon Timestream. \"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \" The time the account was registered, in seconds since epoch (January 1, 1970 at midnight UTC time). \"\n        }\n      ]\n    },\n    \"lastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \" The time this registration was last updated, in seconds since epoch (January 1, 1970 at midnight UTC time). \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"registerAccountStatus\",\n    \"iamResources\",\n    \"creationTime\",\n    \"lastModificationTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-register-account-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: RegisterAccountResponse
---
