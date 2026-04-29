---
description: The AS2 agreement acknowledgement connection settings.
layout: schema
name: AS2AcknowledgementConnectionSettings
properties_list:
- description: Indicates whether to ignore mismatch in certificate name.
  name: ignoreCertificateNameMismatch
  type: boolean
- description: Indicates whether to keep the connection alive.
  name: keepHttpConnectionAlive
  type: boolean
- description: Indicates whether to support HTTP status code 'CONTINUE'.
  name: supportHttpStatusCodeContinue
  type: boolean
- description: Indicates whether to unfold the HTTP headers.
  name: unfoldHttpHeaders
  type: boolean
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-acknowledgement-connection-settings-schema.json
slug: azure-logic-apps-as2-acknowledgement-connection-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-acknowledgement-connection-settings-schema.json\",\n  \"title\": \"AS2AcknowledgementConnectionSettings\",\n  \"description\": \"The AS2 agreement acknowledgement connection settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ignoreCertificateNameMismatch\": {\n      \"description\": \"Indicates whether to ignore mismatch in certificate name.\",\n      \"type\": \"boolean\"\n    },\n    \"keepHttpConnectionAlive\": {\n      \"description\": \"Indicates whether to keep the connection alive.\",\n      \"type\": \"boolean\"\n    },\n    \"supportHttpStatusCodeContinue\": {\n      \"description\": \"Indicates whether to support HTTP status code 'CONTINUE'.\",\n      \"type\": \"boolean\"\n    },\n    \"unfoldHttpHeaders\": {\n      \"description\": \"Indicates whether to\
  \ unfold the HTTP headers.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"ignoreCertificateNameMismatch\",\n    \"supportHttpStatusCodeContinue\",\n    \"keepHttpConnectionAlive\",\n    \"unfoldHttpHeaders\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-acknowledgement-connection-settings-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2AcknowledgementConnectionSettings
---
