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
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2SecuritySettings
---
