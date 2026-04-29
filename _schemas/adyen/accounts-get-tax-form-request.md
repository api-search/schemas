---
description: GetTaxFormRequest schema from Adyen API
layout: schema
name: GetTaxFormRequest
properties_list:
- description: The account holder code you provided when you created the account holder.
  name: accountHolderCode
  type: string
- description: Type of the requested tax form. For example, 1099-K.
  name: formType
  type: string
- description: Applicable tax year in the YYYY format.
  name: year
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-get-tax-form-request-schema.json
slug: accounts-get-tax-form-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-get-tax-form-request-schema.json\",\n  \"title\": \"GetTaxFormRequest\",\n  \"description\": \"GetTaxFormRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The account holder code you provided when you created the account holder.\",\n      \"type\": \"string\"\n    },\n    \"formType\": {\n      \"description\": \"Type of the requested tax form. For example, 1099-K.\",\n      \"type\": \"string\"\n    },\n    \"year\": {\n      \"description\": \"Applicable tax year in the YYYY format.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"formType\",\n    \"year\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-get-tax-form-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetTaxFormRequest
---
