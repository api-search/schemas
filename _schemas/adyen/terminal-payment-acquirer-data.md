---
description: Data related to the response from the payment Acquirer.
layout: schema
name: PaymentAcquirerData
properties_list:
- description: If several Acquirers.
  name: AcquirerID
  type: integer
- description: Identification of the Merchant for the Acquirer.
  name: MerchantID
  type: string
- description: Identification of the POI for the payment Acquirer.
  name: AcquirerPOIID
  type: string
- description: ''
  name: AcquirerTransactionID
  type: object
- description: If available.
  name: ApprovalCode
  type: string
- description: ''
  name: HostReconciliationID
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-acquirer-data-schema.json
slug: terminal-payment-acquirer-data
source_filename: terminal-payment-acquirer-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-acquirer-data-schema.json\",\n  \"title\": \"PaymentAcquirerData\",\n  \"description\": \"Data related to the response from the payment Acquirer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcquirerID\": {\n      \"type\": \"integer\",\n      \"description\": \"If several Acquirers.\"\n    },\n    \"MerchantID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Identification of the Merchant for the Acquirer.\"\n    },\n    \"AcquirerPOIID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Identification of the POI for the payment Acquirer.\"\n    },\n    \"AcquirerTransactionID\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    },\n    \"ApprovalCode\": {\n      \"type\": \"string\",\n  \
  \    \"pattern\": \"^.+$\",\n      \"description\": \"If available.\"\n    },\n    \"HostReconciliationID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"MerchantID\",\n    \"AcquirerPOIID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-acquirer-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentAcquirerData
---
