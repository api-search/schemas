---
description: A FreeRTOS software configuration specifying firmware libraries, settings, and target hardware platform.
layout: schema
name: SoftwareConfiguration
properties_list:
- description: Unique ID of the software configuration.
  name: softwareConfigurationId
  type: string
- description: Name of the software configuration.
  name: name
  type: string
- description: Optional description.
  name: description
  type: string
- description: ARN of the software configuration.
  name: arn
  type: string
- description: Status of the configuration.
  name: status
  type: string
- description: Version string.
  name: version
  type: string
- description: Target microcontroller platform (e.g., ESP32, STM32).
  name: hardwarePlatform
  type: string
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdatedDate
  type: string
provider_name: Amazon FreeRTOS
provider_slug: amazon-freertos
schema_file: json-schema/amazon-freertos-software-configuration-schema.json
slug: amazon-freertos-software-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-software-configuration-schema.json\",\n  \"title\": \"SoftwareConfiguration\",\n  \"description\": \"A FreeRTOS software configuration specifying firmware libraries, settings, and target hardware platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"softwareConfigurationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID of the software configuration.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the software configuration.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the software configuration.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n     \
  \ \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\"\n      ],\n      \"description\": \"Status of the configuration.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version string.\"\n    },\n    \"hardwarePlatform\": {\n      \"type\": \"string\",\n      \"description\": \"Target microcontroller platform (e.g., ESP32, STM32).\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"hardwarePlatform\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-software-configuration-schema.json
tags:
- AWS
- Embedded Systems
- IoT
- Microcontrollers
- RTOS
title: SoftwareConfiguration
---
