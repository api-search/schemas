---
description: BankAccountIdentificationValidationRequest schema from Adyen API
layout: schema
name: BankAccountIdentificationValidationRequest
properties_list:
- description: Bank account identification.
  name: accountIdentification
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-bank-account-identification-validation-request-schema.json
slug: configuration-bank-account-identification-validation-request
source_filename: configuration-bank-account-identification-validation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-bank-account-identification-validation-request-schema.json\",\n  \"title\": \"BankAccountIdentificationValidationRequest\",\n  \"description\": \"BankAccountIdentificationValidationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIdentification\": {\n      \"description\": \"Bank account identification.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AULocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/BRLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CALocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CZLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/DKLocalAccountIdentification\"\
  \n        },\n        {\n          \"$ref\": \"#/components/schemas/HKLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/HULocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/IbanAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NOLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NZLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/NumberAndBicAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/PLLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/SELocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/SGLocalAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/UKLocalAccountIdentification\"\n        },\n   \
  \     {\n          \"$ref\": \"#/components/schemas/USLocalAccountIdentification\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountIdentification\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-bank-account-identification-validation-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccountIdentificationValidationRequest
---
