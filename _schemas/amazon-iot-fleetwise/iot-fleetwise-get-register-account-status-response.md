---
description: GetRegisterAccountStatusResponse schema
layout: schema
name: GetRegisterAccountStatusResponse
properties_list:
- description: ''
  name: customerAccountId
  type: object
- description: ''
  name: accountStatus
  type: object
- description: ''
  name: timestreamRegistrationResponse
  type: object
- description: ''
  name: iamRegistrationResponse
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: lastModificationTime
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-get-register-account-status-response-schema.json
slug: iot-fleetwise-get-register-account-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-register-account-status-response-schema.json\",\n  \"title\": \"GetRegisterAccountStatusResponse\",\n  \"description\": \"GetRegisterAccountStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/customerAccountId\"\n        },\n        {\n          \"description\": \" The unique ID of the Amazon Web Services account, provided at account creation. \"\n        }\n      ]\n    },\n    \"accountStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \"<p> The status of registering your account and resources. The status can be one of:</p> <ul> <li> <p> <code>REGISTRATION_SUCCESS</code>\
  \ - The Amazon Web Services resource is successfully registered.</p> </li> <li> <p> <code>REGISTRATION_PENDING</code> - Amazon Web Services IoT FleetWise is processing the registration request. This process takes approximately five minutes to complete.</p> </li> <li> <p> <code>REGISTRATION_FAILURE</code> - Amazon Web Services IoT FleetWise can't register the AWS resource. Try again later.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"timestreamRegistrationResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamRegistrationResponse\"\n        },\n        {\n          \"description\": \" Information about the registered Amazon Timestream resources or errors, if any.\"\n        }\n      ]\n    },\n    \"iamRegistrationResponse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRegistrationResponse\"\n        },\n        {\n          \"description\": \" Information about the registered IAM resources or errors,\
  \ if any. \"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \" The time the account was registered, in seconds since epoch (January 1, 1970 at midnight UTC time). \"\n        }\n      ]\n    },\n    \"lastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \" The time this registration was last updated, in seconds since epoch (January 1, 1970 at midnight UTC time). \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"customerAccountId\",\n    \"accountStatus\",\n    \"iamRegistrationResponse\",\n    \"creationTime\",\n    \"lastModificationTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-register-account-status-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: GetRegisterAccountStatusResponse
---
