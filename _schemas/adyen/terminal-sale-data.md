---
description: Data associated to the Sale System, with a particular value during the processing of the payment by the POI, including the cards acquisition. Data related to the Sale System.
layout: schema
name: SaleData
properties_list:
- description: ''
  name: OperatorID
  type: string
- description: if different from the Login.
  name: OperatorLanguage
  type: string
- description: if different from the Login and see Login .SaleData.
  name: ShiftNumber
  type: string
- description: ''
  name: SaleTransactionID
  type: object
- description: If payment reservation.
  name: SaleReferenceID
  type: string
- description: ''
  name: SaleTerminalData
  type: object
- description: ''
  name: TokenRequestedType
  type: object
- description: Additional and optional identification of a customer order.
  name: CustomerOrderID
  type: string
- description: ''
  name: CustomerOrderReq
  type: object
- description: Stored with the transaction.
  name: SaleToPOIData
  type: string
- description: Send to the Acquirer if present.
  name: SaleToAcquirerData
  type: string
- description: ''
  name: SaleToIssuerData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sale-data-schema.json
slug: terminal-sale-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-data-schema.json\",\n  \"title\": \"SaleData\",\n  \"description\": \"Data associated to the Sale System, with a particular value during the processing of the payment by the POI, including the cards acquisition. Data related to the Sale System.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OperatorID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"OperatorLanguage\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\",\n      \"description\": \"if different from the Login.\"\n    },\n    \"ShiftNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"if different from the Login and  see Login .SaleData.\"\n    },\n    \"SaleTransactionID\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n\
  \    },\n    \"SaleReferenceID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If payment reservation.\"\n    },\n    \"SaleTerminalData\": {\n      \"$ref\": \"#/components/schemas/SaleTerminalData\"\n    },\n    \"TokenRequestedType\": {\n      \"$ref\": \"#/components/schemas/TokenRequestedType\"\n    },\n    \"CustomerOrderID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Additional and optional identification of a customer order.\"\n    },\n    \"CustomerOrderReq\": {\n      \"$ref\": \"#/components/schemas/CustomerOrderReq\"\n    },\n    \"SaleToPOIData\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Stored with the transaction.\"\n    },\n    \"SaleToAcquirerData\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Send to the Acquirer if present.\"\n    },\n    \"SaleToIssuerData\": {\n      \"$ref\": \"#/components/schemas/SaleToIssuerData\"\
  \n    }\n  },\n  \"required\": [\n    \"SaleTransactionID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SaleData
---
