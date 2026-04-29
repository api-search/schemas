---
description: It conveys Information related to the Sale to POI protocol management. Message header of the Sale to POI protocol message.
layout: schema
name: MessageHeader
properties_list:
- description: If MessageCategory is Login or Diagnosis.
  name: ProtocolVersion
  type: string
- description: ''
  name: MessageClass
  type: object
- description: ''
  name: MessageCategory
  type: object
- description: ''
  name: MessageType
  type: object
- description: Required if Service or Event MessageClass message or if Device MessageClass and request from POI or response from Sale.
  name: ServiceID
  type: string
- description: If Device MessageClass.
  name: DeviceID
  type: string
- description: Identification of a Sale System or a Sale Terminal for the Sale to POI protocol.
  name: SaleID
  type: string
- description: Identification of a POI System or a POI Terminal for the Sale to POI protocol.
  name: POIID
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-message-header-schema.json
slug: terminal-message-header
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-message-header-schema.json\",\n  \"title\": \"MessageHeader\",\n  \"description\": \"It conveys Information related to the Sale to POI protocol management. Message header of the Sale to POI protocol message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProtocolVersion\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If MessageCategory is Login or Diagnosis.\"\n    },\n    \"MessageClass\": {\n      \"$ref\": \"#/components/schemas/MessageClass\"\n    },\n    \"MessageCategory\": {\n      \"$ref\": \"#/components/schemas/MessageCategory\"\n    },\n    \"MessageType\": {\n      \"$ref\": \"#/components/schemas/MessageType\"\n    },\n    \"ServiceID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{1,10}$\",\n      \"description\": \"Required if\
  \ Service or Event MessageClass message or if Device MessageClass and request from POI or response from Sale.\"\n    },\n    \"DeviceID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{1,10}$\",\n      \"description\": \"If Device MessageClass.\"\n    },\n    \"SaleID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Identification of a Sale System or a Sale Terminal for the Sale to POI protocol.\"\n    },\n    \"POIID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Identification of a POI System or a POI Terminal for the Sale to POI protocol.\"\n    }\n  },\n  \"required\": [\n    \"MessageClass\",\n    \"MessageCategory\",\n    \"MessageType\",\n    \"SaleID\",\n    \"POIID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-message-header-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MessageHeader
---
