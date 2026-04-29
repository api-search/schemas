---
description: Object for details about the acquiring institution (for example, merchant bank) or its agent. This includes acquirerIca, acquirerMerchantId and acquirerBin. This object may be used to improve transaction acceptance rates.
layout: schema
name: AcquirerData
properties_list:
- description: An Acquirer Interbank Card Association (ICA) value is an identifier assigned to the Acquirer by Mastercard.
  name: acquirerIca
  type: string
- description: 'Each Acquirer Interbank Card Association (ICA) identifier may be assigned one or more BINs by Mastercard. Note: It is important to use the correct Acquirer ICA associated with the Acquirer BIN.'
  name: acquirerBin
  type: string
- description: A Merchant Identifier (MID) is a unique code assigned to the Merchant by the Acquirer once the Merchant has successfully opened an account. A MID identifies the Merchant to the Acquirer.
  name: acquirerMerchantId
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-checkout-solutions-acquirer-data-schema.json
slug: mastercard-checkout-solutions-acquirer-data
source_filename: mastercard-checkout-solutions-acquirer-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AcquirerData\",\n  \"type\": \"object\",\n  \"description\": \"\\nObject for details about the acquiring institution (for example, merchant bank) or its agent. This includes acquirerIca, acquirerMerchantId and acquirerBin. This object may be used to improve transaction acceptance rates.\\n\",\n  \"properties\": {\n    \"acquirerIca\": {\n      \"type\": \"string\",\n      \"description\": \"An Acquirer Interbank Card Association (ICA) value is an identifier assigned to the Acquirer by Mastercard.\"\n    },\n    \"acquirerBin\": {\n      \"type\": \"string\",\n      \"description\": \"Each Acquirer Interbank Card Association (ICA) identifier may be assigned one or more BINs by Mastercard.\\n\\nNote: It is important to use the correct Acquirer ICA associated with the Acquirer BIN.\\n\"\n    },\n    \"acquirerMerchantId\": {\n      \"type\": \"string\",\n      \"description\": \"A Merchant Identifier\
  \ (MID) is a unique code assigned to the Merchant by the Acquirer once the Merchant has successfully opened an account. A MID identifies the Merchant to the Acquirer.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-checkout-solutions-acquirer-data-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AcquirerData
---
