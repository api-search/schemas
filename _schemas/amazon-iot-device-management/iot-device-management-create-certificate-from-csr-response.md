---
description: The output from the CreateCertificateFromCsr operation.
layout: schema
name: CreateCertificateFromCsrResponse
properties_list:
- description: ''
  name: certificateArn
  type: object
- description: ''
  name: certificateId
  type: object
- description: ''
  name: certificatePem
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-certificate-from-csr-response-schema.json
slug: iot-device-management-create-certificate-from-csr-response
source_filename: iot-device-management-create-certificate-from-csr-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-certificate-from-csr-response-schema.json\",\n  \"title\": \"CreateCertificateFromCsrResponse\",\n  \"description\": \"The output from the CreateCertificateFromCsr operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the certificate. You can use the ARN as a principal for policy operations.\"\n        }\n      ]\n    },\n    \"certificateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateId\"\n        },\n        {\n          \"description\": \"The ID of the certificate. Certificate management operations only\
  \ take a certificateId.\"\n        }\n      ]\n    },\n    \"certificatePem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificatePem\"\n        },\n        {\n          \"description\": \"The certificate data, in PEM format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-certificate-from-csr-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateCertificateFromCsrResponse
---
