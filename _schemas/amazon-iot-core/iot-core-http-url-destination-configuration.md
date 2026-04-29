---
description: HTTP URL destination configuration used by the topic rule's HTTP action.
layout: schema
name: HttpUrlDestinationConfiguration
properties_list:
- description: ''
  name: confirmationUrl
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-http-url-destination-configuration-schema.json
slug: iot-core-http-url-destination-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-http-url-destination-configuration-schema.json\",\n  \"title\": \"HttpUrlDestinationConfiguration\",\n  \"description\": \"HTTP URL destination configuration used by the topic rule's HTTP action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"confirmationUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The URL IoT uses to confirm ownership of or access to the topic rule destination URL.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"confirmationUrl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-http-url-destination-configuration-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: HttpUrlDestinationConfiguration
---
