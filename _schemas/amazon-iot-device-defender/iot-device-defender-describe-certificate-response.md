---
description: The output of the DescribeCertificate operation.
layout: schema
name: DescribeCertificateResponse
properties_list:
- description: ''
  name: certificateDescription
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-certificate-response-schema.json
slug: iot-device-defender-describe-certificate-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-certificate-response-schema.json\",\n  \"title\": \"DescribeCertificateResponse\",\n  \"description\": \"The output of the DescribeCertificate operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateDescription\"\n        },\n        {\n          \"description\": \"The description of the certificate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-certificate-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeCertificateResponse
---
