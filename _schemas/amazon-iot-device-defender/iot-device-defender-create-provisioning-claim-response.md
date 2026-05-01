---
description: CreateProvisioningClaimResponse schema
layout: schema
name: CreateProvisioningClaimResponse
properties_list:
- description: ''
  name: certificateId
  type: object
- description: ''
  name: certificatePem
  type: object
- description: ''
  name: keyPair
  type: object
- description: ''
  name: expiration
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-provisioning-claim-response-schema.json
slug: iot-device-defender-create-provisioning-claim-response
source_filename: iot-device-defender-create-provisioning-claim-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-provisioning-claim-response-schema.json\",\n  \"title\": \"CreateProvisioningClaimResponse\",\n  \"description\": \"CreateProvisioningClaimResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateId\"\n        },\n        {\n          \"description\": \"The ID of the certificate.\"\n        }\n      ]\n    },\n    \"certificatePem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificatePem\"\n        },\n        {\n          \"description\": \"The provisioning claim certificate.\"\n        }\n      ]\n    },\n    \"keyPair\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyPair\"\n\
  \        },\n        {\n          \"description\": \"The provisioning claim key pair.\"\n        }\n      ]\n    },\n    \"expiration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The provisioning claim expiration time.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-provisioning-claim-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateProvisioningClaimResponse
---
