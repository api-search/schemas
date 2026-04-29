---
description: The AS2 agreement envelope settings.
layout: schema
name: AS2EnvelopeSettings
properties_list:
- description: The value indicating whether to auto generate file name.
  name: autogenerateFileName
  type: boolean
- description: The template for file name.
  name: fileNameTemplate
  type: string
- description: The message content type.
  name: messageContentType
  type: string
- description: The value indicating whether to suspend message on file name generation error.
  name: suspendMessageOnFileNameGenerationError
  type: boolean
- description: The value indicating whether to transmit file name in mime header.
  name: transmitFileNameInMimeHeader
  type: boolean
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-envelope-settings-schema.json
slug: azure-logic-apps-as2-envelope-settings
source_filename: azure-logic-apps-as2-envelope-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-envelope-settings-schema.json\",\n  \"title\": \"AS2EnvelopeSettings\",\n  \"description\": \"The AS2 agreement envelope settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"autogenerateFileName\": {\n      \"description\": \"The value indicating whether to auto generate file name.\",\n      \"type\": \"boolean\"\n    },\n    \"fileNameTemplate\": {\n      \"description\": \"The template for file name.\",\n      \"type\": \"string\"\n    },\n    \"messageContentType\": {\n      \"description\": \"The message content type.\",\n      \"type\": \"string\"\n    },\n    \"suspendMessageOnFileNameGenerationError\": {\n      \"description\": \"The value indicating whether to suspend message on file name generation error.\",\n      \"type\": \"boolean\"\n    },\n    \"transmitFileNameInMimeHeader\"\
  : {\n      \"description\": \"The value indicating whether to transmit file name in mime header.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"messageContentType\",\n    \"transmitFileNameInMimeHeader\",\n    \"fileNameTemplate\",\n    \"suspendMessageOnFileNameGenerationError\",\n    \"autogenerateFileName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-envelope-settings-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2EnvelopeSettings
---
