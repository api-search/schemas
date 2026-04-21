---
description: The AS2 agreement validation settings.
layout: schema
name: AS2ValidationSettings
properties_list:
- description: The value indicating whether to check for certificate revocation list on receive.
  name: checkCertificateRevocationListOnReceive
  type: boolean
- description: The value indicating whether to check for certificate revocation list on send.
  name: checkCertificateRevocationListOnSend
  type: boolean
- description: The value indicating whether to check for duplicate message.
  name: checkDuplicateMessage
  type: boolean
- description: The value indicating whether the message has to be compressed.
  name: compressMessage
  type: boolean
- description: The value indicating whether the message has to be encrypted.
  name: encryptMessage
  type: boolean
- description: The encryption algorithm.
  name: encryptionAlgorithm
  type: object
- description: The number of days to look back for duplicate interchange.
  name: interchangeDuplicatesValidityDays
  type: integer
- description: The value indicating whether to override incoming message properties with those in agreement.
  name: overrideMessageProperties
  type: boolean
- description: The value indicating whether the message has to be signed.
  name: signMessage
  type: boolean
- description: The signing algorithm.
  name: signingAlgorithm
  type: object
provider_name: Azure Logic Apps
provider_slug: azure-logic-apps
schema_file: json-schema/azure-logic-apps-as2-validation-settings-schema.json
slug: azure-logic-apps-as2-validation-settings
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2ValidationSettings
---
