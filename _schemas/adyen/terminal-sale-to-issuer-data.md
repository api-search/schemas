---
description: The POI System receives this information and sends it to the Acquirer for the Issuer without any change. Sale information intended for the Issuer.
layout: schema
name: SaleToIssuerData
properties_list:
- description: Information to print on the bank statement.
  name: StatementReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sale-to-issuer-data-schema.json
slug: terminal-sale-to-issuer-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-to-issuer-data-schema.json\",\n  \"title\": \"SaleToIssuerData\",\n  \"description\": \"The POI System receives this information and sends it to the Acquirer for the Issuer without any change. Sale information intended for the Issuer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StatementReference\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Information to print on the bank statement.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-to-issuer-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SaleToIssuerData
---
