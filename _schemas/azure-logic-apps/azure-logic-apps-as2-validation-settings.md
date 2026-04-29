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
source_filename: azure-logic-apps-as2-validation-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-validation-settings-schema.json\",\n  \"title\": \"AS2ValidationSettings\",\n  \"description\": \"The AS2 agreement validation settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkCertificateRevocationListOnReceive\": {\n      \"description\": \"The value indicating whether to check for certificate revocation list on receive.\",\n      \"type\": \"boolean\"\n    },\n    \"checkCertificateRevocationListOnSend\": {\n      \"description\": \"The value indicating whether to check for certificate revocation list on send.\",\n      \"type\": \"boolean\"\n    },\n    \"checkDuplicateMessage\": {\n      \"description\": \"The value indicating whether to check for duplicate message.\",\n      \"type\": \"boolean\"\n    },\n    \"compressMessage\": {\n      \"description\"\
  : \"The value indicating whether the message has to be compressed.\",\n      \"type\": \"boolean\"\n    },\n    \"encryptMessage\": {\n      \"description\": \"The value indicating whether the message has to be encrypted.\",\n      \"type\": \"boolean\"\n    },\n    \"encryptionAlgorithm\": {\n      \"$ref\": \"#/definitions/EncryptionAlgorithm\",\n      \"description\": \"The encryption algorithm.\"\n    },\n    \"interchangeDuplicatesValidityDays\": {\n      \"description\": \"The number of days to look back for duplicate interchange.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"overrideMessageProperties\": {\n      \"description\": \"The value indicating whether to override incoming message properties with those in agreement.\",\n      \"type\": \"boolean\"\n    },\n    \"signMessage\": {\n      \"description\": \"The value indicating whether the message has to be signed.\",\n      \"type\": \"boolean\"\n    },\n    \"signingAlgorithm\": {\n      \"$ref\"\
  : \"#/definitions/SigningAlgorithm\",\n      \"description\": \"The signing algorithm.\"\n    }\n  },\n  \"required\": [\n    \"overrideMessageProperties\",\n    \"encryptMessage\",\n    \"signMessage\",\n    \"compressMessage\",\n    \"checkDuplicateMessage\",\n    \"interchangeDuplicatesValidityDays\",\n    \"checkCertificateRevocationListOnSend\",\n    \"checkCertificateRevocationListOnReceive\",\n    \"encryptionAlgorithm\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-logic-apps/refs/heads/main/json-schema/azure-logic-apps-as2-validation-settings-schema.json
tags:
- Azure
- Integration
- iPaaS
- Workflows
title: AS2ValidationSettings
---
