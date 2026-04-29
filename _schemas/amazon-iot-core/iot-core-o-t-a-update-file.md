---
description: Describes a file to be associated with an OTA update.
layout: schema
name: OTAUpdateFile
properties_list:
- description: ''
  name: fileName
  type: object
- description: ''
  name: fileType
  type: object
- description: ''
  name: fileVersion
  type: object
- description: ''
  name: fileLocation
  type: object
- description: ''
  name: codeSigning
  type: object
- description: ''
  name: attributes
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-o-t-a-update-file-schema.json
slug: iot-core-o-t-a-update-file
source_filename: iot-core-o-t-a-update-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-o-t-a-update-file-schema.json\",\n  \"title\": \"OTAUpdateFile\",\n  \"description\": \"Describes a file to be associated with an OTA update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileName\"\n        },\n        {\n          \"description\": \"The name of the file.\"\n        }\n      ]\n    },\n    \"fileType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileType\"\n        },\n        {\n          \"description\": \"An integer value you can include in the job document to allow your devices to identify the type of file received from the cloud.\"\n        }\n      ]\n    },\n    \"fileVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OTAUpdateFileVersion\"\
  \n        },\n        {\n          \"description\": \"The file version.\"\n        }\n      ]\n    },\n    \"fileLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileLocation\"\n        },\n        {\n          \"description\": \"The location of the updated firmware.\"\n        }\n      ]\n    },\n    \"codeSigning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeSigning\"\n        },\n        {\n          \"description\": \"The code signing method of the file.\"\n        }\n      ]\n    },\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributesMap\"\n        },\n        {\n          \"description\": \"A list of name/attribute pairs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-o-t-a-update-file-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: OTAUpdateFile
---
