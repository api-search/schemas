---
description: The output of the DescribeCertificate operation.
layout: schema
name: DescribeCertificateResponse
properties_list:
- description: ''
  name: certificateDescription
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-certificate-response-schema.json
slug: iot-core-describe-certificate-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-certificate-response-schema.json\",\n  \"title\": \"DescribeCertificateResponse\",\n  \"description\": \"The output of the DescribeCertificate operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateDescription\"\n        },\n        {\n          \"description\": \"The description of the certificate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-certificate-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeCertificateResponse
---
