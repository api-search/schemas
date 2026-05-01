---
description: Represents a collection of device types.
layout: schema
name: DevicePool
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: rules
  type: object
- description: ''
  name: maxDevices
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-device-pool-schema.json
slug: amazon-device-farm-device-pool
source_filename: amazon-device-farm-device-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-device-pool-schema.json\",\n  \"title\": \"DevicePool\",\n  \"description\": \"Represents a collection of device types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The device pool's ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The device pool's name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The device pool's description.\"\n \
  \       }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevicePoolType\"\n        },\n        {\n          \"description\": \"<p>The device pool's type.</p> <p>Allowed values include:</p> <ul> <li> <p>CURATED: A device pool that is created and managed by AWS Device Farm.</p> </li> <li> <p>PRIVATE: A device pool that is created and managed by the device pool developer.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rules\"\n        },\n        {\n          \"description\": \"Information about the device pool's rules.\"\n        }\n      ]\n    },\n    \"maxDevices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"<p>The number of devices that Device Farm can add to your device pool. Device Farm adds devices that are available and meet the criteria\
  \ that you assign for the <code>rules</code> parameter. Depending on how many devices meet these constraints, your device pool might contain fewer devices than the value for this parameter.</p> <p>By specifying the maximum number of devices, you can control the costs that you incur by running tests.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-device-pool-schema.json
tags:
- Application Testing
- Device Testing
- Mobile Testing
- Quality Assurance
title: DevicePool
---
