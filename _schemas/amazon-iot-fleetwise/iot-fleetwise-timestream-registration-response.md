---
description: Information about the registered Amazon Timestream resources or errors, if any.
layout: schema
name: TimestreamRegistrationResponse
properties_list:
- description: ''
  name: timestreamDatabaseName
  type: object
- description: ''
  name: timestreamTableName
  type: object
- description: ''
  name: timestreamDatabaseArn
  type: object
- description: ''
  name: timestreamTableArn
  type: object
- description: ''
  name: registrationStatus
  type: object
- description: ''
  name: errorMessage
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-timestream-registration-response-schema.json
slug: iot-fleetwise-timestream-registration-response
source_filename: iot-fleetwise-timestream-registration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-timestream-registration-response-schema.json\",\n  \"title\": \"TimestreamRegistrationResponse\",\n  \"description\": \"Information about the registered Amazon Timestream resources or errors, if any.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestreamDatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamDatabaseName\"\n        },\n        {\n          \"description\": \"The name of the Timestream database.\"\n        }\n      ]\n    },\n    \"timestreamTableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamTableName\"\n        },\n        {\n          \"description\": \"The name of the Timestream database table.\"\n        }\n      ]\n    },\n    \"timestreamDatabaseArn\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Timestream database.\"\n        }\n      ]\n    },\n    \"timestreamTableArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \"The ARN of the Timestream database table.\"\n        }\n      ]\n    },\n    \"registrationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \"The status of registering your Amazon Timestream resources. The status can be one of <code>REGISTRATION_SUCCESS</code>, <code>REGISTRATION_PENDING</code>, <code>REGISTRATION_FAILURE</code>.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/errorMessage\"\n        },\n        {\n\
  \          \"description\": \"A message associated with a registration error.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timestreamDatabaseName\",\n    \"timestreamTableName\",\n    \"registrationStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-timestream-registration-response-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: TimestreamRegistrationResponse
---
