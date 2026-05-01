---
description: The output of the ListCertificatesByCA operation.
layout: schema
name: ListCertificatesByCAResponse
properties_list:
- description: ''
  name: certificates
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-certificates-by-c-a-response-schema.json
slug: iot-device-defender-list-certificates-by-c-a-response
source_filename: iot-device-defender-list-certificates-by-c-a-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-certificates-by-c-a-response-schema.json\",\n  \"title\": \"ListCertificatesByCAResponse\",\n  \"description\": \"The output of the ListCertificatesByCA operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Certificates\"\n        },\n        {\n          \"description\": \"The device certificates signed by the specified CA certificate.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"The marker for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-certificates-by-c-a-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListCertificatesByCAResponse
---
