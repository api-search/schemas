---
description: A firmware file included in a FreeRTOS OTA update job.
layout: schema
name: OtaFile
properties_list:
- description: Name of the OTA file on the device.
  name: fileName
  type: string
- description: Version of the firmware file.
  name: fileVersion
  type: string
- description: S3 or Stream location of the firmware binary.
  name: fileLocation
  type: object
- description: Code signing configuration for the firmware file.
  name: codeSigning
  type: object
- description: User-defined file type (0-255).
  name: fileType
  type: integer
provider_name: Amazon FreeRTOS
provider_slug: amazon-freertos
schema_file: json-schema/amazon-freertos-ota-file-schema.json
slug: amazon-freertos-ota-file
source_filename: amazon-freertos-ota-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-ota-file-schema.json\",\n  \"title\": \"OtaFile\",\n  \"description\": \"A firmware file included in a FreeRTOS OTA update job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the OTA file on the device.\"\n    },\n    \"fileVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the firmware file.\"\n    },\n    \"fileLocation\": {\n      \"type\": \"object\",\n      \"description\": \"S3 or Stream location of the firmware binary.\"\n    },\n    \"codeSigning\": {\n      \"type\": \"object\",\n      \"description\": \"Code signing configuration for the firmware file.\"\n    },\n    \"fileType\": {\n      \"type\": \"integer\",\n      \"description\": \"User-defined file type (0-255).\"\
  \n    }\n  },\n  \"required\": [\n    \"fileName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-freertos/refs/heads/main/json-schema/amazon-freertos-ota-file-schema.json
tags:
- AWS
- Embedded Systems
- IoT
- Microcontrollers
- RTOS
title: OtaFile
---
