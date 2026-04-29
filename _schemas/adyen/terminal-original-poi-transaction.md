---
description: In the Payment or the Loyalty Request message, it allows using the card of a previous CardAcquisition or Payment/Loyalty request. Identification of a previous POI transaction.
layout: schema
name: OriginalPOITransaction
properties_list:
- description: Identification of a Sale System or a Sale Terminal for the Sale to POI protocol.
  name: SaleID
  type: string
- description: If original transaction is coming from another POI.
  name: POIID
  type: string
- description: ''
  name: POITransactionID
  type: object
- description: Indicate if the card data has to be got from a previous transaction.
  name: ReuseCardDataFlag
  type: boolean
- description: If referral.
  name: ApprovalCode
  type: string
- description: If the language is selected by the Sale System before the request to the POI.
  name: CustomerLanguage
  type: string
- description: Restrict to these Acquirer if present.
  name: AcquirerID
  type: integer
- description: ''
  name: AmountValue
  type: number
- description: ''
  name: HostTransactionID
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-original-poi-transaction-schema.json
slug: terminal-original-poi-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-original-poi-transaction-schema.json\",\n  \"title\": \"OriginalPOITransaction\",\n  \"description\": \"In the Payment or the Loyalty Request message, it allows using the card of a previous CardAcquisition or Payment/Loyalty request. Identification of a previous POI transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SaleID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Identification of a Sale System or a Sale Terminal for the Sale to POI protocol.\"\n    },\n    \"POIID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If original transaction is coming from another POI.\"\n    },\n    \"POITransactionID\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    },\n    \"ReuseCardDataFlag\":\
  \ {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Indicate if the card data has to be got from a previous transaction.\"\n    },\n    \"ApprovalCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If referral.\"\n    },\n    \"CustomerLanguage\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\",\n      \"description\": \"If the language is selected by the Sale System before the request to the POI.\"\n    },\n    \"AcquirerID\": {\n      \"type\": \"integer\",\n      \"description\": \"Restrict to these Acquirer if present.\"\n    },\n    \"AmountValue\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"HostTransactionID\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-original-poi-transaction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OriginalPOITransaction
---
