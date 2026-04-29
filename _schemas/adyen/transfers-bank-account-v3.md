---
description: BankAccountV3 schema from Adyen API
layout: schema
name: BankAccountV3
properties_list:
- description: Information about the owner of the bank account.
  name: accountHolder
  type: object
- description: Contains the bank account details. The fields required in this object depend on the country of the bank account and the currency of the transfer.
  name: accountIdentification
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-bank-account-v3-schema.json
slug: transfers-bank-account-v3
source_filename: transfers-bank-account-v3-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-bank-account-v3-schema.json\",\n  \"title\": \"BankAccountV3\",\n  \"description\": \"BankAccountV3 schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"description\": \"Information about the owner of the bank account.\",\n      \"$ref\": \"#/components/schemas/PartyIdentification\"\n    },\n    \"accountIdentification\": {\n      \"description\": \"Contains the bank account details. The fields required in this object depend on the country of the bank account and the currency of the transfer.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AULocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/BRLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CALocalAccountIdentification\"\
  \n        },\n        {\n          \"$ref\": \"#/components/schemas/CZLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/DKLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/HKLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/HULocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/IbanAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NOLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NZLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NumberAndBicAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/PLLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/SELocalAccountIdentification\"\n        },\n   \
  \     {\n          \"$ref\": \"#/components/schemas/SGLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/UKLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/USLocalAccountIdentification\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountIdentification\",\n    \"accountHolder\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-bank-account-v3-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccountV3
---
