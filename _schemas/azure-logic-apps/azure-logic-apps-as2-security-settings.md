---
description: The AS2 agreement security settings.
layout: schema
name: AS2SecuritySettings
properties_list:
- description: The value indicating whether to enable NRR for inbound decoded messages.
  name: enableNRRForInboundDecodedMessages
  type: boolean
- description: The value indicating whether to enable NRR for inbound encoded messages.
  name: enableNRRForInboundEncodedMessages
  type: boolean
- description: The value indicating whether to enable NRR for inbound MDN.
  name: enableNRRForInboundMDN
  type: boolean
- description: The value indicating whether to enable NRR for outbound decoded messages.
  name: enableNRRForOutboundDecodedMessages
  type: boolean
- description: The value indicating whether to enable NRR for outbound encoded messages.
  name: enableNRRForOutboundEncodedMessages
  type: boolean
- description: The value indicating whether to enable NRR for outbound MDN.
  name: enableNRRForOutboundMDN
  type: boolean
- description: The name of the encryption certificate.
  name: encryptionCertificateName
  type: string
- description: The value indicating whether to send or request a MDN.
  name: overrideGroupSigningCertificate
  type: boolean
- description: The Sha2 algorithm format. Valid values are Sha2, ShaHashSize, ShaHyphenHashSize, Sha2UnderscoreHashSize.
  name: sha2AlgorithmFormat
  type: string
- description: The name of the signing certificate.
  name: signingCertificateName
  type: string
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-security-settings-schema.json
slug: azure-logic-apps-as2-security-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-security-settings-schema.json\",\n  \"title\": \"AS2SecuritySettings\",\n  \"description\": \"The AS2 agreement security settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enableNRRForInboundDecodedMessages\": {\n      \"description\": \"The value indicating whether to enable NRR for inbound decoded messages.\",\n      \"type\": \"boolean\"\n    },\n    \"enableNRRForInboundEncodedMessages\": {\n      \"description\": \"The value indicating whether to enable NRR for inbound encoded messages.\",\n      \"type\": \"boolean\"\n    },\n    \"enableNRRForInboundMDN\": {\n      \"description\": \"The value indicating whether to enable NRR for inbound MDN.\",\n      \"type\": \"boolean\"\n    },\n    \"enableNRRForOutboundDecodedMessages\": {\n      \"description\": \"The\
  \ value indicating whether to enable NRR for outbound decoded messages.\",\n      \"type\": \"boolean\"\n    },\n    \"enableNRRForOutboundEncodedMessages\": {\n      \"description\": \"The value indicating whether to enable NRR for outbound encoded messages.\",\n      \"type\": \"boolean\"\n    },\n    \"enableNRRForOutboundMDN\": {\n      \"description\": \"The value indicating whether to enable NRR for outbound MDN.\",\n      \"type\": \"boolean\"\n    },\n    \"encryptionCertificateName\": {\n      \"description\": \"The name of the encryption certificate.\",\n      \"type\": \"string\"\n    },\n    \"overrideGroupSigningCertificate\": {\n      \"description\": \"The value indicating whether to send or request a MDN.\",\n      \"type\": \"boolean\"\n    },\n    \"sha2AlgorithmFormat\": {\n      \"description\": \"The Sha2 algorithm format. Valid values are Sha2, ShaHashSize, ShaHyphenHashSize, Sha2UnderscoreHashSize.\",\n      \"type\": \"string\"\n    },\n    \"signingCertificateName\"\
  : {\n      \"description\": \"The name of the signing certificate.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"overrideGroupSigningCertificate\",\n    \"enableNRRForInboundEncodedMessages\",\n    \"enableNRRForInboundDecodedMessages\",\n    \"enableNRRForOutboundMDN\",\n    \"enableNRRForOutboundEncodedMessages\",\n    \"enableNRRForOutboundDecodedMessages\",\n    \"enableNRRForInboundMDN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-security-settings-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2SecuritySettings
---
