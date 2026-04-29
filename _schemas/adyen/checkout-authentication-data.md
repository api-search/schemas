---
description: AuthenticationData schema from Adyen API
layout: schema
name: AuthenticationData
properties_list:
- description: 'Indicates when 3D Secure authentication should be attempted. This overrides all other rules, including [Dynamic 3D Secure settings](https://docs.adyen.com/risk-management/dynamic-3d-secure). Possible '
  name: attemptAuthentication
  type: string
- description: If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation. Default
  name: authenticationOnly
  type: boolean
- description: Object with additional parameters for the 3D Secure authentication flow.
  name: threeDSRequestData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-authentication-data-schema.json
slug: checkout-authentication-data
source_filename: checkout-authentication-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-authentication-data-schema.json\",\n  \"title\": \"AuthenticationData\",\n  \"description\": \"AuthenticationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attemptAuthentication\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Indicates when 3D Secure authentication should be attempted. This overrides all other rules, including [Dynamic 3D Secure settings](https://docs.adyen.com/risk-management/dynamic-3d-secure).\\n\\nPossible values:\\n\\n* **always**: Perform 3D Secure authentication.\\n* **never**: Don't perform 3D Secure authentication. If PSD2 SCA or other national regulations require authentication, the transaction gets declined.\",\n      \"enum\": [\n        \"always\",\n        \"never\"\n      ],\n      \"type\": \"string\"\n    },\n    \"\
  authenticationOnly\": {\n      \"x-addedInVersion\": \"69\",\n      \"default\": false,\n      \"description\": \"If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation.\\nDefault: **false**.\",\n      \"type\": \"boolean\"\n    },\n    \"threeDSRequestData\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Object with additional parameters for the 3D Secure authentication flow.\",\n      \"$ref\": \"#/components/schemas/ThreeDSRequestData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-authentication-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthenticationData
---
