---
description: Acquirer reference ID & card acceptor ID pair
layout: schema
name: AcquirerMerchantId
properties_list:
- description: Marks the ARID/CAID pair as relevant for the FPT engine. When false, the FPT engine won't use the ARID/CAID pair for identifying transactions.
  name: firstPartyTrustEnabled
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-acquirer-merchant-id-schema.json
slug: mastercard-ethoca-merchant-self-services-acquirer-merchant-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AcquirerMerchantId\",\n  \"type\": \"object\",\n  \"description\": \"Acquirer reference ID & card acceptor ID pair\",\n  \"properties\": {\n    \"firstPartyTrustEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Marks the ARID/CAID pair as relevant for the FPT engine. When false, the FPT engine won't use the ARID/CAID pair for identifying transactions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-acquirer-merchant-id-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AcquirerMerchantId
---
