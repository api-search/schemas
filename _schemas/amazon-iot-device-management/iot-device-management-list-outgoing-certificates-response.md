---
description: The output from the ListOutgoingCertificates operation.
layout: schema
name: ListOutgoingCertificatesResponse
properties_list:
- description: ''
  name: outgoingCertificates
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-outgoing-certificates-response-schema.json
slug: iot-device-management-list-outgoing-certificates-response
source_filename: iot-device-management-list-outgoing-certificates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-outgoing-certificates-response-schema.json\",\n  \"title\": \"ListOutgoingCertificatesResponse\",\n  \"description\": \"The output from the ListOutgoingCertificates operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"outgoingCertificates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutgoingCertificates\"\n        },\n        {\n          \"description\": \"The certificates that are being transferred but not yet accepted.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"The marker for the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-outgoing-certificates-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListOutgoingCertificatesResponse
---
