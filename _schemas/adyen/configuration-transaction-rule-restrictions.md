---
description: TransactionRuleRestrictions schema from Adyen API
layout: schema
name: TransactionRuleRestrictions
properties_list:
- description: 'The total number of tokens that a card can have across different kinds of digital wallets on the user''s phones, watches, or other wearables. Supported operations: **equals**, **notEquals**, **greaterT'
  name: activeNetworkTokens
  type: object
- description: 'List of card brand variants and the operation. Supported operations: **anyMatch**, **noneMatch**.'
  name: brandVariants
  type: object
- description: 'List of counterparty Institutions and the operation. Supported operations: **anyMatch**, **noneMatch**.'
  name: counterpartyBank
  type: object
- description: 'List of countries and the operation. Supported operations: **anyMatch**, **noneMatch**.'
  name: countries
  type: object
- description: 'List of week days and the operation. Supported operations: **anyMatch**, **noneMatch**.'
  name: dayOfWeek
  type: object
- description: 'Compares the currency of the payment against the currency of the payment instrument, and specifies the operation. Supported operations: **equals**, **notEquals**.'
  name: differentCurrencies
  type: object
- description: 'List of point-of-sale entry modes and the operation.. Supported operations: **anyMatch**, **noneMatch**.'
  name: entryModes
  type: object
- description: 'Indicates whether transaction is an international transaction and specifies the operation. Supported operations: **equals**, **notEquals**.'
  name: internationalTransaction
  type: object
- description: 'The number of transactions and the operation. Supported operations: **equals**, **notEquals**, **greaterThanOrEqualTo**, **greaterThan**, **lessThanOrEqualTo**, **lessThan**.'
  name: matchingTransactions
  type: object
- description: 'List of merchant category codes (MCCs) and the operation. Supported operations: **anyMatch**, **noneMatch**.'
  name: mccs
  type: object
- description: 'List of names that will be compared to the merchant name according to the matching type. Supported operations: **anyMatch**, **noneMatch**.'
  name: merchantNames
  type: object
- description: 'List of merchant ID and acquirer ID pairs, and the operation. Supported operations: **anyMatch**, **noneMatch**.'
  name: merchants
  type: object
- description: 'List of processing types and the operation. Supported operations: **anyMatch**, **noneMatch**.'
  name: processingTypes
  type: object
- description: 'Checks if a user has recently sent the same amount of funds in multiple transfers. To use this restriction, you must: - Set the rule `type` to **velocity**. - Specify a time `interval`. - Specify a nu'
  name: sameAmountRestriction
  type: object
- description: 'Checks if a user has recently made multiple transfers to the same counterparty. To use this restriction, you must: - Set the rule `type` to **velocity**. - Specify a time `interval`. - Specify a numbe'
  name: sameCounterpartyRestriction
  type: object
- description: 'A start and end time in a time-only ISO-8601 extended offset format. Supported operations: **equals**, **notEquals**.'
  name: timeOfDay
  type: object
- description: 'The total amount and the operation. Supported operations: **equals**, **notEquals**, **greaterThanOrEqualTo**, **greaterThan**, **lessThanOrEqualTo**, **lessThan**.'
  name: totalAmount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transaction-rule-restrictions-schema.json
slug: configuration-transaction-rule-restrictions
source_filename: configuration-transaction-rule-restrictions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-restrictions-schema.json\",\n  \"title\": \"TransactionRuleRestrictions\",\n  \"description\": \"TransactionRuleRestrictions schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activeNetworkTokens\": {\n      \"description\": \"The total number of tokens that a card can have across different kinds of digital wallets on the user's phones, watches, or other wearables.\\n\\nSupported operations: **equals**, **notEquals**, **greaterThanOrEqualTo**, **greaterThan**, **lessThanOrEqualTo**, **lessThan**.\",\n      \"$ref\": \"#/components/schemas/ActiveNetworkTokensRestriction\"\n    },\n    \"brandVariants\": {\n      \"description\": \"List of card brand variants and the operation.\\n\\nSupported operations: **anyMatch**, **noneMatch**.\",\n      \"$ref\": \"#/components/schemas/BrandVariantsRestriction\"\
  \n    },\n    \"counterpartyBank\": {\n      \"description\": \"List of counterparty Institutions and the operation. Supported operations: **anyMatch**, **noneMatch**.\",\n      \"$ref\": \"#/components/schemas/CounterpartyBankRestriction\"\n    },\n    \"countries\": {\n      \"description\": \"List of countries and the operation.\\n\\nSupported operations: **anyMatch**, **noneMatch**.\",\n      \"$ref\": \"#/components/schemas/CountriesRestriction\"\n    },\n    \"dayOfWeek\": {\n      \"description\": \"List of week days and the operation. Supported operations: **anyMatch**, **noneMatch**.\",\n      \"$ref\": \"#/components/schemas/DayOfWeekRestriction\"\n    },\n    \"differentCurrencies\": {\n      \"description\": \"Compares the currency of the payment against the currency of the payment instrument, and specifies the operation.\\n\\nSupported operations: **equals**, **notEquals**.\",\n      \"$ref\": \"#/components/schemas/DifferentCurrenciesRestriction\"\n    },\n    \"entryModes\"\
  : {\n      \"description\": \"List of point-of-sale entry modes and the operation..\\n\\nSupported operations: **anyMatch**, **noneMatch**.\",\n      \"$ref\": \"#/components/schemas/EntryModesRestriction\"\n    },\n    \"internationalTransaction\": {\n      \"description\": \"Indicates whether transaction is an international transaction and specifies the operation.\\n\\nSupported operations: **equals**, **notEquals**.\",\n      \"$ref\": \"#/components/schemas/InternationalTransactionRestriction\"\n    },\n    \"matchingTransactions\": {\n      \"description\": \"The number of transactions and the operation.\\n\\nSupported operations: **equals**, **notEquals**, **greaterThanOrEqualTo**, **greaterThan**, **lessThanOrEqualTo**, **lessThan**.\",\n      \"$ref\": \"#/components/schemas/MatchingTransactionsRestriction\"\n    },\n    \"mccs\": {\n      \"description\": \"List of merchant category codes (MCCs) and the operation.\\n\\nSupported operations: **anyMatch**, **noneMatch**.\",\n  \
  \    \"$ref\": \"#/components/schemas/MccsRestriction\"\n    },\n    \"merchantNames\": {\n      \"description\": \"List of names that will be compared to the merchant name according to the matching type.\\n\\nSupported operations: **anyMatch**, **noneMatch**.\",\n      \"$ref\": \"#/components/schemas/MerchantNamesRestriction\"\n    },\n    \"merchants\": {\n      \"description\": \"List of merchant ID and acquirer ID pairs, and the operation.\\n\\nSupported operations: **anyMatch**, **noneMatch**.\",\n      \"$ref\": \"#/components/schemas/MerchantsRestriction\"\n    },\n    \"processingTypes\": {\n      \"description\": \"List of processing types and the operation.\\n\\nSupported operations: **anyMatch**, **noneMatch**.\",\n      \"$ref\": \"#/components/schemas/ProcessingTypesRestriction\"\n    },\n    \"sameAmountRestriction\": {\n      \"description\": \"Checks if a user has recently sent the same amount of funds in multiple transfers.\\n\\nTo use this restriction, you must:\\n\\\
  n- Set the rule `type` to **velocity**.\\n\\n- Specify a time `interval`.\\n\\n- Specify a number of `matchingTransactions`.\\n\\nSupported operation: **equals**.\",\n      \"$ref\": \"#/components/schemas/SameAmountRestriction\"\n    },\n    \"sameCounterpartyRestriction\": {\n      \"description\": \"Checks if a user has recently made multiple transfers to the same counterparty.\\n\\nTo use this restriction, you must:\\n\\n- Set the rule `type` to **velocity**.\\n\\n- Specify a time `interval`.\\n\\n- Specify a number of `matchingTransactions`.\\n\\nSupported operations: **equals**.\",\n      \"$ref\": \"#/components/schemas/SameCounterpartyRestriction\"\n    },\n    \"timeOfDay\": {\n      \"description\": \"A start and end time in a time-only ISO-8601 extended offset format. Supported operations: **equals**, **notEquals**.\",\n      \"$ref\": \"#/components/schemas/TimeOfDayRestriction\"\n    },\n    \"totalAmount\": {\n      \"description\": \"The total amount and the operation.\\\
  n\\nSupported operations: **equals**, **notEquals**, **greaterThanOrEqualTo**, **greaterThan**, **lessThanOrEqualTo**, **lessThan**.\",\n      \"$ref\": \"#/components/schemas/TotalAmountRestriction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-restrictions-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRuleRestrictions
---
