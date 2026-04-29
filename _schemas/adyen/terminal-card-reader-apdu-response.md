---
description: It contains the result of the requested service, APDU response sent by the chip of the card in response to the APDU request. Content of the Card Reader APDU Response message.
layout: schema
name: CardReaderAPDUResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: Data field of the APDU command (Lc + Data).
  name: APDUData
  type: string
- description: Status of a smartcard response to a command (SW1-SW2).
  name: CardStatusWords
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-card-reader-apdu-response-schema.json
slug: terminal-card-reader-apdu-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-reader-apdu-response-schema.json\",\n  \"title\": \"CardReaderAPDUResponse\",\n  \"description\": \"It contains the result of the requested service, APDU response sent by the chip of the card in response to the APDU request. Content of the Card Reader APDU Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"APDUData\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Data field of the APDU command (Lc + Data).\"\n    },\n    \"CardStatusWords\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.{2,2}$\",\n      \"description\": \"Status of a smartcard response to a command (SW1-SW2).\"\n    }\n  },\n\
  \  \"required\": [\n    \"Response\",\n    \"CardStatusWords\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-reader-apdu-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardReaderAPDUResponse
---
