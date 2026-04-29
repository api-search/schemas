---
description: The integration account AS2 one-way agreement.
layout: schema
name: AS2OneWayAgreement
properties_list:
- description: The AS2 protocol settings.
  name: protocolSettings
  type: object
- description: The receiver business identity
  name: receiverBusinessIdentity
  type: object
- description: The sender business identity
  name: senderBusinessIdentity
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-one-way-agreement-schema.json
slug: azure-logic-apps-as2-one-way-agreement
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-one-way-agreement-schema.json\",\n  \"title\": \"AS2OneWayAgreement\",\n  \"description\": \"The integration account AS2 one-way agreement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"protocolSettings\": {\n      \"$ref\": \"#/definitions/AS2ProtocolSettings\",\n      \"description\": \"The AS2 protocol settings.\"\n    },\n    \"receiverBusinessIdentity\": {\n      \"$ref\": \"#/definitions/BusinessIdentity\",\n      \"description\": \"The receiver business identity\"\n    },\n    \"senderBusinessIdentity\": {\n      \"$ref\": \"#/definitions/BusinessIdentity\",\n      \"description\": \"The sender business identity\"\n    }\n  },\n  \"required\": [\n    \"senderBusinessIdentity\",\n    \"receiverBusinessIdentity\",\n    \"protocolSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-one-way-agreement-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2OneWayAgreement
---
