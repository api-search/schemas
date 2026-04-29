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
source_filename: azure-logic-apps-as2-mdn-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-mdn-settings-schema.json\",\n  \"title\": \"AS2MdnSettings\",\n  \"description\": \"The AS2 agreement mdn settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dispositionNotificationTo\": {\n      \"description\": \"The disposition notification to header value.\",\n      \"type\": \"string\"\n    },\n    \"mdnText\": {\n      \"description\": \"The MDN text.\",\n      \"type\": \"string\"\n    },\n    \"micHashingAlgorithm\": {\n      \"$ref\": \"#/definitions/HashingAlgorithm\",\n      \"description\": \"The signing or hashing algorithm.\"\n    },\n    \"needMDN\": {\n      \"description\": \"The value indicating whether to send or request a MDN.\",\n      \"type\": \"boolean\"\n    },\n    \"receiptDeliveryUrl\": {\n      \"description\": \"The receipt delivery URL.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"sendInboundMDNToMessageBox\": {\n      \"description\": \"The value indicating whether to send inbound MDN to message box.\",\n      \"type\": \"boolean\"\n    },\n    \"sendMDNAsynchronously\": {\n      \"description\": \"The value indicating whether to send the asynchronous MDN.\",\n      \"type\": \"boolean\"\n    },\n    \"signMDN\": {\n      \"description\": \"The value indicating whether the MDN needs to be signed or not.\",\n      \"type\": \"boolean\"\n    },\n    \"signOutboundMDNIfOptional\": {\n      \"description\": \"The value indicating whether to sign the outbound MDN if optional.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"needMDN\",\n    \"signMDN\",\n    \"sendMDNAsynchronously\",\n    \"signOutboundMDNIfOptional\",\n    \"sendInboundMDNToMessageBox\",\n    \"micHashingAlgorithm\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-mdn-settings-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2MdnSettings
---
