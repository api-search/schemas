---
description: The AS2 agreement protocol settings.
layout: schema
name: AS2ProtocolSettings
properties_list:
- description: The acknowledgement connection settings.
  name: acknowledgementConnectionSettings
  type: object
- description: The envelope settings.
  name: envelopeSettings
  type: object
- description: The error settings.
  name: errorSettings
  type: object
- description: The MDN settings.
  name: mdnSettings
  type: object
- description: The message connection settings.
  name: messageConnectionSettings
  type: object
- description: The security settings.
  name: securitySettings
  type: object
- description: The validation settings.
  name: validationSettings
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-protocol-settings-schema.json
slug: azure-logic-apps-as2-protocol-settings
source_filename: azure-logic-apps-as2-protocol-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-protocol-settings-schema.json\",\n  \"title\": \"AS2ProtocolSettings\",\n  \"description\": \"The AS2 agreement protocol settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acknowledgementConnectionSettings\": {\n      \"$ref\": \"#/definitions/AS2AcknowledgementConnectionSettings\",\n      \"description\": \"The acknowledgement connection settings.\"\n    },\n    \"envelopeSettings\": {\n      \"$ref\": \"#/definitions/AS2EnvelopeSettings\",\n      \"description\": \"The envelope settings.\"\n    },\n    \"errorSettings\": {\n      \"$ref\": \"#/definitions/AS2ErrorSettings\",\n      \"description\": \"The error settings.\"\n    },\n    \"mdnSettings\": {\n      \"$ref\": \"#/definitions/AS2MdnSettings\",\n      \"description\": \"The MDN settings.\"\n    },\n    \"\
  messageConnectionSettings\": {\n      \"$ref\": \"#/definitions/AS2MessageConnectionSettings\",\n      \"description\": \"The message connection settings.\"\n    },\n    \"securitySettings\": {\n      \"$ref\": \"#/definitions/AS2SecuritySettings\",\n      \"description\": \"The security settings.\"\n    },\n    \"validationSettings\": {\n      \"$ref\": \"#/definitions/AS2ValidationSettings\",\n      \"description\": \"The validation settings.\"\n    }\n  },\n  \"required\": [\n    \"messageConnectionSettings\",\n    \"acknowledgementConnectionSettings\",\n    \"mdnSettings\",\n    \"securitySettings\",\n    \"validationSettings\",\n    \"envelopeSettings\",\n    \"errorSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-protocol-settings-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2ProtocolSettings
---
