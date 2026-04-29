---
description: BankAccountInfo schema from Adyen API
layout: schema
name: BankAccountInfo
properties_list:
- description: Identification of the bank account.
  name: accountIdentification
  type: object
- description: The type of bank account.
  name: accountType
  type: string
- description: The name of the banking institution where the bank account is held.
  name: bankName
  type: string
- description: The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code where the bank account is registered. For example, **NL**.
  name: countryCode
  type: string
- description: Identifies if the bank account was created through [instant bank verification](https://docs.adyen.com/release-notes/platforms-and-financial-products#releaseNote=2023-05-08-hosted-onboarding).
  name: trustedSource
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-bank-account-info-schema.json
slug: legal-entity-bank-account-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-bank-account-info-schema.json\",\n  \"title\": \"BankAccountInfo\",\n  \"description\": \"BankAccountInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIdentification\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Identification of the bank account.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AULocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CALocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CZLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/DKLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/HKLocalAccountIdentification\"\n\
  \        },\n        {\n          \"$ref\": \"#/components/schemas/HULocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/IbanAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NOLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NZLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NumberAndBicAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/PLLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/SELocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/SGLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/UKLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/USLocalAccountIdentification\"\n        }\n     \
  \ ]\n    },\n    \"accountType\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"2\",\n      \"description\": \"The type of bank account.\",\n      \"type\": \"string\"\n    },\n    \"bankName\": {\n      \"description\": \"The name of the banking institution where the bank account is held.\",\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"description\": \"The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code where the bank account is registered. For example, **NL**.\",\n      \"type\": \"string\"\n    },\n    \"trustedSource\": {\n      \"description\": \"Identifies if the bank account was created through [instant bank verification](https://docs.adyen.com/release-notes/platforms-and-financial-products#releaseNote=2023-05-08-hosted-onboarding).\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-bank-account-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccountInfo
---
