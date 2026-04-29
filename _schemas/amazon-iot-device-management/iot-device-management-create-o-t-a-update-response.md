---
description: CreateOTAUpdateResponse schema
layout: schema
name: CreateOTAUpdateResponse
properties_list:
- description: ''
  name: otaUpdateId
  type: object
- description: ''
  name: awsIotJobId
  type: object
- description: ''
  name: otaUpdateArn
  type: object
- description: ''
  name: awsIotJobArn
  type: object
- description: ''
  name: otaUpdateStatus
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-o-t-a-update-response-schema.json
slug: iot-device-management-create-o-t-a-update-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-o-t-a-update-response-schema.json\",\n  \"title\": \"CreateOTAUpdateResponse\",\n  \"description\": \"CreateOTAUpdateResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"otaUpdateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OTAUpdateId\"\n        },\n        {\n          \"description\": \"The OTA update ID.\"\n        }\n      ]\n    },\n    \"awsIotJobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsIotJobId\"\n        },\n        {\n          \"description\": \"The IoT job ID associated with the OTA update.\"\n        }\n      ]\n    },\n    \"otaUpdateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OTAUpdateArn\"\n        },\n  \
  \      {\n          \"description\": \"The OTA update ARN.\"\n        }\n      ]\n    },\n    \"awsIotJobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsIotJobArn\"\n        },\n        {\n          \"description\": \"The IoT job ARN associated with the OTA update.\"\n        }\n      ]\n    },\n    \"otaUpdateStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OTAUpdateStatus\"\n        },\n        {\n          \"description\": \"The OTA update status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-o-t-a-update-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateOTAUpdateResponse
---
