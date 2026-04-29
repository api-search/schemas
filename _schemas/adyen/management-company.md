---
description: Company schema from Adyen API
layout: schema
name: Company
properties_list:
- description: References to resources connected with this company.
  name: _links
  type: object
- description: List of available data centers. Adyen has several data centers around the world.In the URL that you use for making API requests, we recommend you use the live URL prefix from the data center closest t
  name: dataCenters
  type: array
- description: Your description for the company account, maximum 300 characters
  name: description
  type: string
- description: The unique identifier of the company account.
  name: id
  type: string
- description: The legal or trading name of the company.
  name: name
  type: string
- description: Your reference to the account
  name: reference
  type: string
- description: 'The status of the company account. Possible values: * **Active**: Users can log in. Processing and payout capabilities depend on the status of the merchant account. * **Inactive**: Users can log in. P'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-company-schema.json
slug: management-company
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-company-schema.json\",\n  \"title\": \"Company\",\n  \"description\": \"Company schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"description\": \"References to resources connected with this company.\",\n      \"$ref\": \"#/components/schemas/CompanyLinks\"\n    },\n    \"dataCenters\": {\n      \"description\": \"List of available data centers.\\n\\nAdyen has several data centers around the world.In the URL that you use for making API requests, we recommend you use the live URL prefix from the data center closest to your shoppers.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DataCenter\"\n      },\n      \"type\": \"array\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the company account, maximum 300\
  \ characters\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the company account.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The legal or trading name of the company.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference to the account\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the company account.\\n\\nPossible values:\\n\\n* **Active**: Users can log in. Processing and payout capabilities depend on the status of the merchant account.\\n* **Inactive**: Users can log in. Payment processing and payouts are disabled.\\n* **Closed**: The company account is closed and this cannot be reversed. Users cannot log in. Payment processing and payouts are disabled.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-company-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Company
---
