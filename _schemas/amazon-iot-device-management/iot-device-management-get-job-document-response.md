---
description: GetJobDocumentResponse schema
layout: schema
name: GetJobDocumentResponse
properties_list:
- description: ''
  name: document
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-get-job-document-response-schema.json
slug: iot-device-management-get-job-document-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-job-document-response-schema.json\",\n  \"title\": \"GetJobDocumentResponse\",\n  \"description\": \"GetJobDocumentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"document\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDocument\"\n        },\n        {\n          \"description\": \"The job document content.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-job-document-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: GetJobDocumentResponse
---
