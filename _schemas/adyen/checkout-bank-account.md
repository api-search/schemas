---
description: BankAccount schema from Adyen API
layout: schema
name: BankAccount
properties_list:
- description: The bank account number (without separators).
  name: bankAccountNumber
  type: string
- description: The bank city.
  name: bankCity
  type: string
- description: The location id of the bank. The field value is `nil` in most cases.
  name: bankLocationId
  type: string
- description: The name of the bank.
  name: bankName
  type: string
- description: The [Business Identifier Code](https://en.wikipedia.org/wiki/ISO_9362) (BIC) is the SWIFT address assigned to a bank. The field value is `nil` in most cases.
  name: bic
  type: string
- description: Country code where the bank is located. A valid value is an ISO two-character country code (e.g. 'NL').
  name: countryCode
  type: string
- description: The [International Bank Account Number](https://en.wikipedia.org/wiki/International_Bank_Account_Number) (IBAN).
  name: iban
  type: string
- description: The name of the bank account holder. If you submit a name with non-Latin characters, we automatically replace some of them with corresponding Latin characters to meet the FATF recommendations. For exa
  name: ownerName
  type: string
- description: The bank account holder's tax ID.
  name: taxId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-bank-account-schema.json
slug: checkout-bank-account
source_filename: checkout-bank-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-bank-account-schema.json\",\n  \"title\": \"BankAccount\",\n  \"description\": \"BankAccount schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccountNumber\": {\n      \"description\": \"The bank account number (without separators).\",\n      \"type\": \"string\"\n    },\n    \"bankCity\": {\n      \"x-addedInVersion\": \"18\",\n      \"description\": \"The bank city.\",\n      \"type\": \"string\"\n    },\n    \"bankLocationId\": {\n      \"description\": \"The location id of the bank. The field value is `nil` in most cases.\",\n      \"type\": \"string\"\n    },\n    \"bankName\": {\n      \"description\": \"The name of the bank.\",\n      \"type\": \"string\"\n    },\n    \"bic\": {\n      \"description\": \"The [Business Identifier Code](https://en.wikipedia.org/wiki/ISO_9362)\
  \ (BIC) is the SWIFT address assigned to a bank. The field value is `nil` in most cases.\",\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"description\": \"Country code where the bank is located.\\n\\nA valid value is an ISO two-character country code (e.g. 'NL').\",\n      \"type\": \"string\"\n    },\n    \"iban\": {\n      \"description\": \"The [International Bank Account Number](https://en.wikipedia.org/wiki/International_Bank_Account_Number) (IBAN).\",\n      \"type\": \"string\"\n    },\n    \"ownerName\": {\n      \"description\": \"The name of the bank account holder.\\nIf you submit a name with non-Latin characters, we automatically replace some of them with corresponding Latin characters to meet the FATF recommendations. For example:\\n* \\u03c712 is converted to ch12.\\n* \\u00fcA is converted to euA.\\n* Peter M\\u00f8ller is converted to Peter Mller, because banks don't accept '\\u00f8'.\\nAfter replacement, the ownerName must have at least three alphanumeric\
  \ characters (A-Z, a-z, 0-9), and at least one of them must be a valid Latin character (A-Z, a-z). For example:\\n* John17 - allowed.\\n* J17 - allowed.\\n* 171 - not allowed.\\n* John-7 - allowed.\\n> If provided details don't match the required format, the response returns the error message: 203 'Invalid bank account holder name'.\",\n      \"type\": \"string\"\n    },\n    \"taxId\": {\n      \"x-addedInVersion\": \"18\",\n      \"description\": \"The bank account holder's tax ID.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-bank-account-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BankAccount
---
