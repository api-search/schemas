---
description: 'SearchFields is an array of SearchField objects. The following validations apply: * If the searchFields array contains both TRANSACTION_AMOUNT and TRANSACTION_CURRENCY_CODE searchParameters, then the value of the "searchFieldCards" and "required" properties must be same for both items * If the searchFields array contains the TRANSACTION_AMOUNT searchParameter, then it must also contain the TRANSACTION_CURRENCY_CODE searchParameter (and vice versa)'
layout: schema
name: SearchFields
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-search-fields-schema.json
slug: mastercard-ethoca-merchant-self-services-search-fields
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchFields\",\n  \"type\": \"array\",\n  \"description\": \"SearchFields is an array of SearchField objects. The following validations apply:\\n* If the searchFields array contains both TRANSACTION_AMOUNT and TRANSACTION_CURRENCY_CODE searchParameters, then the value of the \\\"searchFieldCards\\\" and \\\"required\\\" properties must be same for both items\\n* If the searchFields array contains the TRANSACTION_AMOUNT searchParameter, then it must also contain the TRANSACTION_CURRENCY_CODE searchParameter (and vice versa)\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-search-fields-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SearchFields
---
