---
description: The output from the GetRegistrationCode operation.
layout: schema
name: GetRegistrationCodeResponse
properties_list:
- description: ''
  name: registrationCode
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-get-registration-code-response-schema.json
slug: iot-core-get-registration-code-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-registration-code-response-schema.json\",\n  \"title\": \"GetRegistrationCodeResponse\",\n  \"description\": \"The output from the GetRegistrationCode operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"registrationCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationCode\"\n        },\n        {\n          \"description\": \"The CA certificate registration code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-registration-code-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: GetRegistrationCodeResponse
---
