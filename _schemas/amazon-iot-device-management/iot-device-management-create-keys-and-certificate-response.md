---
description: The output of the CreateKeysAndCertificate operation.
layout: schema
name: CreateKeysAndCertificateResponse
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
- description: ''
  name: keyPair
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-keys-and-certificate-response-schema.json
slug: iot-device-management-create-keys-and-certificate-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-keys-and-certificate-response-schema.json\",\n  \"title\": \"CreateKeysAndCertificateResponse\",\n  \"description\": \"The output of the CreateKeysAndCertificate operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateArn\"\n        },\n        {\n          \"description\": \"The ARN of the certificate.\"\n        }\n      ]\n    },\n    \"certificateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateId\"\n        },\n        {\n          \"description\": \"The ID of the certificate. IoT issues a default subject name for the certificate (for example, IoT Certificate).\"\n        }\n      ]\n    },\n    \"\
  certificatePem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificatePem\"\n        },\n        {\n          \"description\": \"The certificate data, in PEM format.\"\n        }\n      ]\n    },\n    \"keyPair\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyPair\"\n        },\n        {\n          \"description\": \"The generated key pair.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-keys-and-certificate-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateKeysAndCertificateResponse
---
