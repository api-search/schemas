---
description: To abort a transaction in progress or to request the status of a transaction from which no response has been received. It identifies the message header of the message request to abort or request the status. Identification of a previous POI transaction.
layout: schema
name: MessageReference
properties_list:
- description: ''
  name: MessageCategory
  type: object
- description: Identification of a message pair, which processes a transaction.
  name: ServiceID
  type: string
- description: Identification of a device message pair.
  name: DeviceID
  type: string
- description: default MessageHeader.SaleID.
  name: SaleID
  type: string
- description: default MessageHeader.POIID.
  name: POIID
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-message-reference-schema.json
slug: terminal-message-reference
source_filename: terminal-message-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-message-reference-schema.json\",\n  \"title\": \"MessageReference\",\n  \"description\": \"To abort a transaction in progress or to request the status of a transaction from which no response has been received.  It identifies the message header of the message request to abort or request the status. Identification of a previous POI transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageCategory\": {\n      \"$ref\": \"#/components/schemas/MessageCategory\"\n    },\n    \"ServiceID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{1,10}$\",\n      \"description\": \"Identification of a message pair, which processes a transaction.\"\n    },\n    \"DeviceID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{1,10}$\",\n      \"description\": \"Identification of a device message\
  \ pair.\"\n    },\n    \"SaleID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"default MessageHeader.SaleID.\"\n    },\n    \"POIID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"default MessageHeader.POIID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-message-reference-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MessageReference
---
