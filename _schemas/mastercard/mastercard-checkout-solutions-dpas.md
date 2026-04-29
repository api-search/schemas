---
description: ''
layout: schema
name: Dpas
properties_list:
- description: The registered identifier for the Digital Payment Application (DPA) accessing the service. At least one DPA needs to be registered for each Merchant/Merchant OBO/Sub-Merchant (PF) needed, with additio
  name: srcDpaId
  type: string
- description: Indicates if the Digital Payment Application (DPA) has an Acquirer relationship. This field may be used to improve acceptance rates.
  name: hasAcquirerRelationship
  type: string
- description: Identifier assigned to a Sub-Merchant by the Payment Facilitator (PF). This field may be used to improve transaction security and acceptance rates.
  name: subMerchantId
  type: string
- description: Payment Facilitator (PF) identifier that may be used to improve transaction security and acceptance rates.
  name: paymentFacilitatorId
  type: string
- description: 'Conditional: Must be set to true when the Digital Payment Application (DPA) processes in the United States (US) under the Click to Pay (C2P) program.'
  name: debitTokenRequested
  type: boolean
- description: Object for the array of Merchant Category Codes (MCC) that the Merchant processes transactions under, and is used for risk-scoring transactions by the issuer. All MCC codes that will be processed by a
  name: merchantCategoryCodes
  type: array
- description: ''
  name: acquirerData
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-checkout-solutions-dpas-schema.json
slug: mastercard-checkout-solutions-dpas
source_filename: mastercard-checkout-solutions-dpas-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dpas\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"srcDpaId\": {\n      \"type\": \"string\",\n      \"description\": \"\\nThe registered identifier for the Digital Payment Application (DPA) accessing the service. At least one DPA needs to be registered for each Merchant/Merchant OBO/Sub-Merchant (PF) needed, with additional DPAs being added as required.\\n\\nConditional: Required if you are a Merchant directly integrating with Mastercard Checkout Solutions (MCS) APIs, a Payment Service Provider (PSP) integrating On-Behalf-Of (OBO) a Merchant, a Payment Facilitator, or if you are enrolling in the Secure Card on File (SCOF) QR program.\\n\"\n    },\n    \"hasAcquirerRelationship\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates if the Digital Payment Application (DPA) has an Acquirer relationship. This field may be used to improve acceptance rates.\"\n    },\n  \
  \  \"subMerchantId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier assigned to a Sub-Merchant by the Payment Facilitator (PF). This field may be used to improve transaction security and acceptance rates.\"\n    },\n    \"paymentFacilitatorId\": {\n      \"type\": \"string\",\n      \"description\": \"Payment Facilitator (PF) identifier that may be used to improve transaction security and acceptance rates.\"\n    },\n    \"debitTokenRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Conditional: Must be set to true when the Digital Payment Application (DPA) processes in the United States (US) under the Click to Pay (C2P) program.\\n\"\n    },\n    \"merchantCategoryCodes\": {\n      \"type\": \"array\",\n      \"description\": \"Object for the array of Merchant Category Codes (MCC) that the Merchant processes transactions under, and is used for risk-scoring transactions by the issuer. All MCC codes that will be processed by a DPA should be provided\
  \ here (typically, this will be a single item).\\n\\nAn MCC is a four-character code assigned by Mastercard to the Merchant that indicates the type of business, service, or product provided by the Merchant.\\n\\nNote: MCC's may be assigned differently across payment networks. To avoid errors, be sure to use your assigned Mastercard MCC. This code is required for 3-D Secure (3DS) and risk profiling. If the Merchant has more than one MCC, the code most relevant to their business should be used.\\n\"\n    },\n    \"acquirerData\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-checkout-solutions-dpas-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Dpas
---
