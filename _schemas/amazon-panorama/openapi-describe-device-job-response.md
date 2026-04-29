---
description: DescribeDeviceJobResponse schema from Amazon Panorama
layout: schema
name: DescribeDeviceJobResponse
properties_list:
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: DeviceArn
  type: object
- description: ''
  name: DeviceId
  type: object
- description: ''
  name: DeviceName
  type: object
- description: ''
  name: DeviceType
  type: object
- description: ''
  name: ImageVersion
  type: object
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobType
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-device-job-response-schema.json
slug: openapi-describe-device-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-device-job-response-schema.json\",\n  \"title\": \"DescribeDeviceJobResponse\",\n  \"description\": \"DescribeDeviceJobResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateCreatedTime\"\n        },\n        {\n          \"description\": \"When the job was created.\"\n        }\n      ]\n    },\n    \"DeviceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceArn\"\n        },\n        {\n          \"description\": \"The device's ARN.\"\n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\"\
  : \"The device's ID.\"\n        }\n      ]\n    },\n    \"DeviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceName\"\n        },\n        {\n          \"description\": \"The device's name.\"\n        }\n      ]\n    },\n    \"DeviceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceType\"\n        },\n        {\n          \"description\": \"The device's type.\"\n        }\n      ]\n    },\n    \"ImageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageVersion\"\n        },\n        {\n          \"description\": \"For an OTA job, the target version of the device software.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"The job's type.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateProgress\"\n        },\n        {\n          \"description\": \"The job's status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-device-job-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribeDeviceJobResponse
---
