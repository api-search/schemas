---
description: Set of acquirer reference ID & card acceptor ID pairs resource
layout: schema
name: AcquirerMerchantIdsResource
properties_list:
- description: Rejected acquirer reference ID & card acceptor ID pairs
  name: rejectedIds
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-acquirer-merchant-ids-resource-schema.json
slug: mastercard-ethoca-merchant-self-services-acquirer-merchant-ids-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AcquirerMerchantIdsResource\",\n  \"type\": \"object\",\n  \"description\": \"Set of acquirer reference ID & card acceptor ID pairs resource\",\n  \"properties\": {\n    \"rejectedIds\": {\n      \"type\": \"array\",\n      \"description\": \"Rejected acquirer reference ID & card acceptor ID pairs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-acquirer-merchant-ids-resource-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AcquirerMerchantIdsResource
---
