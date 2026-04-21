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
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2EnvelopeSettings
---
