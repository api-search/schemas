---
description: A container for account-level settings in AWS Device Farm.
layout: schema
name: AccountSettings
properties_list:
- description: ''
  name: awsAccountNumber
  type: object
- description: ''
  name: unmeteredDevices
  type: object
- description: ''
  name: unmeteredRemoteAccessDevices
  type: object
- description: ''
  name: maxJobTimeoutMinutes
  type: object
- description: ''
  name: trialMinutes
  type: object
- description: ''
  name: maxSlots
  type: object
- description: ''
  name: defaultJobTimeoutMinutes
  type: object
- description: ''
  name: skipAppResign
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-account-settings-schema.json
slug: amazon-device-farm-account-settings
source_filename: amazon-device-farm-account-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-account-settings-schema.json\",\n  \"title\": \"AccountSettings\",\n  \"description\": \"A container for account-level settings in AWS Device Farm.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsAccountNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSAccountNumber\"\n        },\n        {\n          \"description\": \"The AWS account number specified in the <code>AccountSettings</code> container.\"\n        }\n      ]\n    },\n    \"unmeteredDevices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PurchasedDevicesMap\"\n        },\n        {\n          \"description\": \"Returns the unmetered devices you have purchased or want to purchase.\"\n        }\n      ]\n    },\n    \"unmeteredRemoteAccessDevices\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PurchasedDevicesMap\"\n        },\n        {\n          \"description\": \"Returns the unmetered remote access devices you have purchased or want to purchase.\"\n        }\n      ]\n    },\n    \"maxJobTimeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTimeoutMinutes\"\n        },\n        {\n          \"description\": \"The maximum number of minutes a test run executes before it times out.\"\n        }\n      ]\n    },\n    \"trialMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrialMinutes\"\n        },\n        {\n          \"description\": \"Information about an AWS account's usage of free trial device minutes.\"\n        }\n      ]\n    },\n    \"maxSlots\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxSlotMap\"\n        },\n        {\n          \"description\": \"The maximum number\
  \ of device slots that the AWS account can purchase. Each maximum is expressed as an <code>offering-id:number</code> pair, where the <code>offering-id</code> represents one of the IDs returned by the <code>ListOfferings</code> command.\"\n        }\n      ]\n    },\n    \"defaultJobTimeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTimeoutMinutes\"\n        },\n        {\n          \"description\": \"The default number of minutes (at the account level) a test run executes before it times out. The default value is 150 minutes.\"\n        }\n      ]\n    },\n    \"skipAppResign\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SkipAppResign\"\n        },\n        {\n          \"description\": \"<p>When set to <code>true</code>, for private devices, Device Farm does not sign your app again. For public devices, Device Farm always signs your apps again.</p> <p>For more information about how Device Farm re-signs your\
  \ apps, see <a href=\\\"http://aws.amazon.com/device-farm/faqs/\\\">Do you modify my app?</a> in the <i>AWS Device Farm FAQs</i>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-account-settings-schema.json
tags:
- Application Testing
- Device Testing
- Mobile Testing
- Quality Assurance
title: AccountSettings
---
