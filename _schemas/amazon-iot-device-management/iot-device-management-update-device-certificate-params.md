---
description: Parameters to define a mitigation action that changes the state of the device certificate to inactive.
layout: schema
name: UpdateDeviceCertificateParams
properties_list:
- description: ''
  name: action
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-update-device-certificate-params-schema.json
slug: iot-device-management-update-device-certificate-params
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-update-device-certificate-params-schema.json\",\n  \"title\": \"UpdateDeviceCertificateParams\",\n  \"description\": \"Parameters to define a mitigation action that changes the state of the device certificate to inactive.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceCertificateUpdateAction\"\n        },\n        {\n          \"description\": \"The action that you want to apply to the device certificate. The only supported value is <code>DEACTIVATE</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-update-device-certificate-params-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: UpdateDeviceCertificateParams
---
