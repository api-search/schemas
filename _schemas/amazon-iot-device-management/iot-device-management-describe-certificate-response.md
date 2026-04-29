---
description: The output of the DescribeCertificate operation.
layout: schema
name: DescribeCertificateResponse
properties_list:
- description: ''
  name: certificateDescription
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-certificate-response-schema.json
slug: iot-device-management-describe-certificate-response
source_filename: iot-device-management-describe-certificate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-certificate-response-schema.json\",\n  \"title\": \"DescribeCertificateResponse\",\n  \"description\": \"The output of the DescribeCertificate operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateDescription\"\n        },\n        {\n          \"description\": \"The description of the certificate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-certificate-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeCertificateResponse
---
