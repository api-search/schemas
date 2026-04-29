---
description: ProvisionDeviceResponse schema from Amazon Panorama
layout: schema
name: ProvisionDeviceResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Certificates
  type: object
- description: ''
  name: DeviceId
  type: object
- description: ''
  name: IotThingName
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-provision-device-response-schema.json
slug: openapi-provision-device-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-provision-device-response-schema.json\",\n  \"title\": \"ProvisionDeviceResponse\",\n  \"description\": \"ProvisionDeviceResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceArn\"\n        },\n        {\n          \"description\": \"The device's ARN.\"\n        }\n      ]\n    },\n    \"Certificates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Certificates\"\n        },\n        {\n          \"description\": \"The device's configuration bundle.\"\n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\": \"\
  The device's ID.\"\n        }\n      ]\n    },\n    \"IotThingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotThingName\"\n        },\n        {\n          \"description\": \"The device's IoT thing name.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceStatus\"\n        },\n        {\n          \"description\": \"The device's status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-provision-device-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ProvisionDeviceResponse
---
