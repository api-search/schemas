---
description: The AS2 agreement error settings.
layout: schema
name: AS2ErrorSettings
properties_list:
- description: The value indicating whether to resend message If MDN is not received.
  name: resendIfMDNNotReceived
  type: boolean
- description: The value indicating whether to suspend duplicate message.
  name: suspendDuplicateMessage
  type: boolean
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-error-settings-schema.json
slug: azure-logic-apps-as2-error-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-error-settings-schema.json\",\n  \"title\": \"AS2ErrorSettings\",\n  \"description\": \"The AS2 agreement error settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resendIfMDNNotReceived\": {\n      \"description\": \"The value indicating whether to resend message If MDN is not received.\",\n      \"type\": \"boolean\"\n    },\n    \"suspendDuplicateMessage\": {\n      \"description\": \"The value indicating whether to suspend duplicate message.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"suspendDuplicateMessage\",\n    \"resendIfMDNNotReceived\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-error-settings-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2ErrorSettings
---
