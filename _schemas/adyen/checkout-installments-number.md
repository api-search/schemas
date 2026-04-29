---
description: InstallmentsNumber schema from Adyen API
layout: schema
name: InstallmentsNumber
properties_list:
- description: Maximum number of installments
  name: maxNumberOfInstallments
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-installments-number-schema.json
slug: checkout-installments-number
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-installments-number-schema.json\",\n  \"title\": \"InstallmentsNumber\",\n  \"description\": \"InstallmentsNumber schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxNumberOfInstallments\": {\n      \"description\": \"Maximum number of installments\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"maxNumberOfInstallments\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-installments-number-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InstallmentsNumber
---
