---
description: Schema for Temenos banking account arrangements including current accounts, savings accounts, deposits, and loans with balance information and product configuration.
layout: schema
name: Temenos Banking Account
properties_list:
- description: Unique account identifier assigned by the Temenos system
  name: accountId
  type: string
- description: Identifier of the customer who owns the account
  name: customerId
  type: string
- description: Display name for the account
  name: accountName
  type: string
- description: Classification of the account type
  name: accountType
  type: string
- description: Product identifier defining the account terms and conditions
  name: productId
  type: string
- description: Account currency in ISO 4217 format
  name: currency
  type: string
- description: Current operational status of the account
  name: status
  type: string
- description: Date the account was opened
  name: openingDate
  type: string
- description: Date the account was closed, null if still active
  name: closingDate
  type:
  - string
  - 'null'
- description: ''
  name: balances
  type: object
- description: Applied interest rate as a percentage
  name: interestRate
  type:
  - number
  - 'null'
- description: Maturity date for term deposits and loans
  name: maturityDate
  type:
  - string
  - 'null'
- description: Branch identifier where the account is held
  name: branchId
  type: string
- description: International Bank Account Number
  name: iban
  type: string
- description: Bank Identifier Code (SWIFT code)
  name: bic
  type: string
provider_name: Temenos
provider_slug: temenos
schema_file: json-schema/temenos-account-schema.json
slug: temenos-account
source_filename: temenos-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://temenos.com/schemas/temenos/account.json\",\n  \"title\": \"Temenos Banking Account\",\n  \"description\": \"Schema for Temenos banking account arrangements including current accounts, savings accounts, deposits, and loans with balance information and product configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"accountId\", \"customerId\", \"accountType\", \"currency\", \"status\"],\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier assigned by the Temenos system\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the customer who owns the account\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the account\",\n      \"maxLength\": 100\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Classification of the account type\",\n      \"enum\": [\"CURRENT\", \"SAVINGS\", \"DEPOSIT\", \"LOAN\", \"MORTGAGE\", \"ISLAMIC\"]\n    },\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Product identifier defining the account terms and conditions\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Account currency in ISO 4217 format\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of the account\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\", \"CLOSED\", \"DORMANT\", \"SUSPENDED\"]\n    },\n    \"openingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the account was opened\"\n    },\n    \"closingDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date the account was closed, null if still active\"\n\
  \    },\n    \"balances\": {\n      \"$ref\": \"#/$defs/AccountBalances\"\n    },\n    \"interestRate\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Applied interest rate as a percentage\",\n      \"minimum\": 0\n    },\n    \"maturityDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Maturity date for term deposits and loans\"\n    },\n    \"branchId\": {\n      \"type\": \"string\",\n      \"description\": \"Branch identifier where the account is held\"\n    },\n    \"iban\": {\n      \"type\": \"string\",\n      \"description\": \"International Bank Account Number\",\n      \"pattern\": \"^[A-Z]{2}[0-9]{2}[A-Z0-9]{4,30}$\"\n    },\n    \"bic\": {\n      \"type\": \"string\",\n      \"description\": \"Bank Identifier Code (SWIFT code)\",\n      \"pattern\": \"^[A-Z]{4}[A-Z]{2}[A-Z0-9]{2}([A-Z0-9]{3})?$\"\n    }\n  },\n  \"$defs\": {\n    \"AccountBalances\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Account balance breakdown across different balance types\",\n      \"properties\": {\n        \"workingBalance\": {\n          \"type\": \"number\",\n          \"description\": \"Current working balance including all posted transactions\"\n        },\n        \"availableBalance\": {\n          \"type\": \"number\",\n          \"description\": \"Balance available for new transactions after holds and limits\"\n        },\n        \"lockedAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Amount currently held or locked for pending operations\",\n          \"minimum\": 0\n        },\n        \"clearedBalance\": {\n          \"type\": \"number\",\n          \"description\": \"Balance of cleared and settled funds only\"\n        },\n        \"pendingDebits\": {\n          \"type\": \"number\",\n          \"description\": \"Sum of pending debit transactions\",\n          \"minimum\": 0\n        },\n        \"pendingCredits\": {\n          \"type\": \"number\",\n \
  \         \"description\": \"Sum of pending credit transactions\",\n          \"minimum\": 0\n        },\n        \"overdraftLimit\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Approved overdraft limit if applicable\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/json-schema/temenos-account-schema.json
tags:
- Banking
- Cloud Banking
- Core Banking
- Digital Banking
- Financial Services
- Fintech
- Open Banking
- Payments
- Wealth Management
title: Temenos Banking Account
---
