---
description: Parameters to define a mitigation action that changes the state of the CA certificate to inactive.
layout: schema
name: UpdateCACertificateParams
properties_list:
- description: ''
  name: action
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-update-c-a-certificate-params-schema.json
slug: iot-core-update-c-a-certificate-params
source_filename: iot-core-update-c-a-certificate-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-update-c-a-certificate-params-schema.json\",\n  \"title\": \"UpdateCACertificateParams\",\n  \"description\": \"Parameters to define a mitigation action that changes the state of the CA certificate to inactive.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CACertificateUpdateAction\"\n        },\n        {\n          \"description\": \"The action that you want to apply to the CA certificate. The only supported value is <code>DEACTIVATE</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-update-c-a-certificate-params-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: UpdateCACertificateParams
---
