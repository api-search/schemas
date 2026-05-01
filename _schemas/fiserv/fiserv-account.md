---
description: Schema representing a financial account across Fiserv banking and card APIs including BankingHub and CardDeveloper.
layout: schema
name: Fiserv Account
properties_list:
- description: The unique account identifier.
  name: accountId
  type: string
- description: The account number.
  name: accountNumber
  type: string
- description: The type of account.
  name: accountType
  type: string
- description: The current account status.
  name: status
  type: string
- description: The party (customer) identifier who owns the account.
  name: partyId
  type: string
- description: The product code for the account.
  name: productCode
  type: string
- description: The branch identifier where the account is held.
  name: branchId
  type: string
- description: The ISO 4217 currency code for the account.
  name: currency
  type: string
- description: ''
  name: balances
  type: object
- description: ''
  name: limits
  type: object
- description: The date the account was opened.
  name: openDate
  type: string
- description: The date the account was closed, if applicable.
  name: closeDate
  type: string
- description: The billing cycle day of the month for credit accounts.
  name: billingCycleDay
  type: integer
provider_name: Fiserv
provider_slug: fiserv
schema_file: json-schema/fiserv-account-schema.json
slug: fiserv-account
source_filename: fiserv-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.fiserv.com/schemas/fiserv/account.json\",\n  \"title\": \"Fiserv Account\",\n  \"description\": \"Schema representing a financial account across Fiserv banking and card APIs including BankingHub and CardDeveloper.\",\n  \"type\": \"object\",\n  \"required\": [\"accountId\", \"accountType\", \"status\"],\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique account identifier.\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The account number.\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"enum\": [\"DDA\", \"SDA\", \"MMA\", \"CDA\", \"LOAN\", \"CONSUMER_CREDIT\", \"COMMERCIAL_CREDIT\", \"CONSUMER_DEBIT\"],\n      \"description\": \"The type of account.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\", \"\
  CLOSED\", \"DORMANT\", \"FROZEN\"],\n      \"description\": \"The current account status.\"\n    },\n    \"partyId\": {\n      \"type\": \"string\",\n      \"description\": \"The party (customer) identifier who owns the account.\"\n    },\n    \"productCode\": {\n      \"type\": \"string\",\n      \"description\": \"The product code for the account.\"\n    },\n    \"branchId\": {\n      \"type\": \"string\",\n      \"description\": \"The branch identifier where the account is held.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"The ISO 4217 currency code for the account.\"\n    },\n    \"balances\": {\n      \"$ref\": \"#/$defs/Balances\"\n    },\n    \"limits\": {\n      \"$ref\": \"#/$defs/Limits\"\n    },\n    \"openDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the account was opened.\"\n    },\n    \"closeDate\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date\",\n      \"description\": \"The date the account was closed, if applicable.\"\n    },\n    \"billingCycleDay\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 28,\n      \"description\": \"The billing cycle day of the month for credit accounts.\"\n    }\n  },\n  \"$defs\": {\n    \"Balances\": {\n      \"type\": \"object\",\n      \"description\": \"Account balance information.\",\n      \"properties\": {\n        \"available\": {\n          \"type\": \"number\",\n          \"description\": \"The available balance or available credit.\"\n        },\n        \"current\": {\n          \"type\": \"number\",\n          \"description\": \"The current (ledger) balance.\"\n        },\n        \"pending\": {\n          \"type\": \"number\",\n          \"description\": \"The pending balance from unposted transactions.\"\n        },\n        \"creditLimit\": {\n          \"type\": \"number\",\n          \"description\": \"The credit limit for credit\
  \ accounts.\"\n        },\n        \"minimumPaymentDue\": {\n          \"type\": \"number\",\n          \"description\": \"The minimum payment due for credit accounts.\"\n        }\n      }\n    },\n    \"Limits\": {\n      \"type\": \"object\",\n      \"description\": \"Account limit information for credit and card accounts.\",\n      \"properties\": {\n        \"creditLimit\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"The permanent credit limit.\"\n        },\n        \"temporaryCreditLimit\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"The temporary credit limit.\"\n        },\n        \"temporaryCreditLimitExpiry\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The expiry date for the temporary credit limit.\"\n        },\n        \"cashLimit\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\":\
  \ \"The cash advance limit.\"\n        },\n        \"availableCredit\": {\n          \"type\": \"number\",\n          \"description\": \"The available credit amount.\"\n        },\n        \"availableCash\": {\n          \"type\": \"number\",\n          \"description\": \"The available cash advance amount.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/json-schema/fiserv-account-schema.json
tags:
- Banking
- Financial
- Payments
- Wealth Management
title: Fiserv Account
---
