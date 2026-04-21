---
description: The AS2 agreement mdn settings.
layout: schema
name: AS2MdnSettings
properties_list:
- description: The disposition notification to header value.
  name: dispositionNotificationTo
  type: string
- description: The MDN text.
  name: mdnText
  type: string
- description: The signing or hashing algorithm.
  name: micHashingAlgorithm
  type: object
- description: The value indicating whether to send or request a MDN.
  name: needMDN
  type: boolean
- description: The receipt delivery URL.
  name: receiptDeliveryUrl
  type: string
- description: The value indicating whether to send inbound MDN to message box.
  name: sendInboundMDNToMessageBox
  type: boolean
- description: The value indicating whether to send the asynchronous MDN.
  name: sendMDNAsynchronously
  type: boolean
- description: The value indicating whether the MDN needs to be signed or not.
  name: signMDN
  type: boolean
- description: The value indicating whether to sign the outbound MDN if optional.
  name: signOutboundMDNIfOptional
  type: boolean
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-mdn-settings-schema.json
slug: azure-logic-apps-as2-mdn-settings
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2MdnSettings
---
