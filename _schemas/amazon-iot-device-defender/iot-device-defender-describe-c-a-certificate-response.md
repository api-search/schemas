---
description: The output from the DescribeCACertificate operation.
layout: schema
name: DescribeCACertificateResponse
properties_list:
- description: ''
  name: certificateDescription
  type: object
- description: ''
  name: registrationConfig
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-c-a-certificate-response-schema.json
slug: iot-device-defender-describe-c-a-certificate-response
source_filename: iot-device-defender-describe-c-a-certificate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-c-a-certificate-response-schema.json\",\n  \"title\": \"DescribeCACertificateResponse\",\n  \"description\": \"The output from the DescribeCACertificate operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CACertificateDescription\"\n        },\n        {\n          \"description\": \"The CA certificate description.\"\n        }\n      ]\n    },\n    \"registrationConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationConfig\"\n        },\n        {\n          \"description\": \"Information about the registration configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-c-a-certificate-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeCACertificateResponse
---
