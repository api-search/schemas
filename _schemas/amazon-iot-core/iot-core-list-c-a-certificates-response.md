---
description: The output from the ListCACertificates operation.
layout: schema
name: ListCACertificatesResponse
properties_list:
- description: ''
  name: certificates
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-c-a-certificates-response-schema.json
slug: iot-core-list-c-a-certificates-response
source_filename: iot-core-list-c-a-certificates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-c-a-certificates-response-schema.json\",\n  \"title\": \"ListCACertificatesResponse\",\n  \"description\": \"The output from the ListCACertificates operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CACertificates\"\n        },\n        {\n          \"description\": \"The CA certificates registered in your Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"The current position within the list of CA certificates.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-c-a-certificates-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: ListCACertificatesResponse
---
