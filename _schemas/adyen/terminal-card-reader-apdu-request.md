---
description: It contains the APDU request to send to the chip of the card, and a possible invitation message to display on the CashierInterface or the CustomerInterface. Content of the Card Reader APDU Request message.
layout: schema
name: CardReaderAPDURequest
properties_list:
- description: Class field of the APDU command (CLA).
  name: APDUClass
  type: string
- description: Instruction field of the APDU command (INS).
  name: APDUInstruction
  type: string
- description: Parameter 1 field of the APDU command (P1).
  name: APDUPar1
  type: string
- description: Parameter 2 field of the APDU command(P2).
  name: APDUPar2
  type: string
- description: Data field of the APDU command (Lc + Data).
  name: APDUData
  type: string
- description: Expected length of the data field of the APDU response to the command (Le).
  name: APDUExpectedLength
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-card-reader-apdu-request-schema.json
slug: terminal-card-reader-apdu-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-reader-apdu-request-schema.json\",\n  \"title\": \"CardReaderAPDURequest\",\n  \"description\": \"It contains the APDU request to send to the chip of the card, and a possible invitation message to display on the CashierInterface or the CustomerInterface. Content of the Card Reader APDU Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"APDUClass\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.{1,1}$\",\n      \"description\": \"Class field of the APDU command (CLA).\"\n    },\n    \"APDUInstruction\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.{1,1}$\",\n      \"description\": \"Instruction field of the APDU command (INS).\"\n    },\n    \"APDUPar1\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"byte\",\n      \"pattern\": \"^.{1,1}$\",\n      \"description\": \"Parameter 1 field of the APDU command (P1).\"\n    },\n    \"APDUPar2\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.{1,1}$\",\n      \"description\": \"Parameter 2 field of the APDU command(P2).\"\n    },\n    \"APDUData\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Data field of the APDU command (Lc + Data).\"\n    },\n    \"APDUExpectedLength\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.{1,1}$\",\n      \"description\": \"Expected length of the data field of the APDU response to the command (Le).\"\n    }\n  },\n  \"required\": [\n    \"APDUClass\",\n    \"APDUInstruction\",\n    \"APDUPar1\",\n    \"APDUPar2\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-reader-apdu-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardReaderAPDURequest
---
