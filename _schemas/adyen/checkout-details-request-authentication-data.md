---
description: DetailsRequestAuthenticationData schema from Adyen API
layout: schema
name: DetailsRequestAuthenticationData
properties_list:
- description: If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation. Default
  name: authenticationOnly
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-details-request-authentication-data-schema.json
slug: checkout-details-request-authentication-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-details-request-authentication-data-schema.json\",\n  \"title\": \"DetailsRequestAuthenticationData\",\n  \"description\": \"DetailsRequestAuthenticationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationOnly\": {\n      \"x-addedInVersion\": \"69\",\n      \"default\": false,\n      \"description\": \"If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation.\\nDefault: *false**.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-details-request-authentication-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DetailsRequestAuthenticationData
---
