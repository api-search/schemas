---
description: Represents the device instance.
layout: schema
name: DeviceInstance
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: deviceArn
  type: object
- description: ''
  name: labels
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: udid
  type: object
- description: ''
  name: instanceProfile
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-device-instance-schema.json
slug: amazon-device-farm-device-instance
source_filename: amazon-device-farm-device-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-device-instance-schema.json\",\n  \"title\": \"DeviceInstance\",\n  \"description\": \"Represents the device instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the device instance.\"\n        }\n      ]\n    },\n    \"deviceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The ARN of the device.\"\n        }\n      ]\n    },\n    \"labels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceLabels\"\n        },\n        {\n          \"description\"\
  : \"An array of strings that describe the device instance.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceStatus\"\n        },\n        {\n          \"description\": \"The status of the device instance. Valid values are listed here.\"\n        }\n      ]\n    },\n    \"udid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique device identifier for the device instance.\"\n        }\n      ]\n    },\n    \"instanceProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceProfile\"\n        },\n        {\n          \"description\": \"A object that contains information about the instance profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-device-instance-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: DeviceInstance
---
