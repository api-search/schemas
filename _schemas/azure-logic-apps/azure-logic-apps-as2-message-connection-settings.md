---
description: The AS2 agreement message connection settings.
layout: schema
name: AS2MessageConnectionSettings
properties_list:
- description: The value indicating whether to ignore mismatch in certificate name.
  name: ignoreCertificateNameMismatch
  type: boolean
- description: The value indicating whether to keep the connection alive.
  name: keepHttpConnectionAlive
  type: boolean
- description: The value indicating whether to support HTTP status code 'CONTINUE'.
  name: supportHttpStatusCodeContinue
  type: boolean
- description: The value indicating whether to unfold the HTTP headers.
  name: unfoldHttpHeaders
  type: boolean
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-message-connection-settings-schema.json
slug: azure-logic-apps-as2-message-connection-settings
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2MessageConnectionSettings
---
