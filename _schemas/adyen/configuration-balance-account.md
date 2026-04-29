---
description: BalanceAccount schema from Adyen API
layout: schema
name: BalanceAccount
properties_list:
- description: The unique identifier of the [account holder](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/accountHolders__resParam_id) associated with the balance account.
  name: accountHolderId
  type: string
- description: List of balances with the amount and currency.
  name: balances
  type: array
- description: The default three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes) of the balance account. The default value is **EUR**. > After a balance account is created,
  name: defaultCurrencyCode
  type: string
- description: A human-readable description of the balance account, maximum 300 characters. You can use this parameter to distinguish between multiple balance accounts under an account holder.
  name: description
  type: string
- description: The unique identifier of the balance account.
  name: id
  type: string
- description: A set of key and value pairs for general use. The keys do not have specific names and may be used for storing miscellaneous data as desired. > Note that during an update of metadata, the omission of e
  name: metadata
  type: object
- description: The unique identifier of the account of the migrated account holder in the classic integration.
  name: migratedAccountCode
  type: string
- description: Contains key-value pairs to the configure the settlement model in a balance account.
  name: platformPaymentConfiguration
  type: object
- description: Your reference for the balance account, maximum 150 characters.
  name: reference
  type: string
- description: The status of the balance account, set to **active** by default.
  name: status
  type: string
- description: The time zone of the balance account. For example, **Europe/Amsterdam**. Defaults to the time zone of the account holder if no time zone is set. For possible values, see the [list of time zone codes](
  name: timeZone
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-balance-account-schema.json
slug: configuration-balance-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-account-schema.json\",\n  \"title\": \"BalanceAccount\",\n  \"description\": \"BalanceAccount schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderId\": {\n      \"description\": \"The unique identifier of the [account holder](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/accountHolders__resParam_id) associated with the balance account.\",\n      \"type\": \"string\"\n    },\n    \"balances\": {\n      \"description\": \"List of balances with the amount and currency.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Balance\"\n      },\n      \"type\": \"array\"\n    },\n    \"defaultCurrencyCode\": {\n      \"description\": \"The default three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes)\
  \ of the balance account.\\nThe default value is **EUR**.\\n> After a balance account is created, you cannot change its default currency.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"A human-readable description of the balance account, maximum 300 characters. You can use this parameter to distinguish between multiple balance accounts under an account holder.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the balance account.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of key and value pairs for general use.\\nThe keys do not have specific names and may be used for storing miscellaneous data as desired.\\n> Note that during an update of metadata, the omission of existing key-value pairs will result in the deletion of those key-value pairs.\"\
  ,\n      \"type\": \"object\"\n    },\n    \"migratedAccountCode\": {\n      \"description\": \"The unique identifier of the account of the migrated account holder in the classic integration.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"platformPaymentConfiguration\": {\n      \"description\": \"Contains key-value pairs to the configure the settlement model in a balance account.\",\n      \"$ref\": \"#/components/schemas/PlatformPaymentConfiguration\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the balance account, maximum 150 characters.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the balance account, set to **active** by default. \\n\",\n      \"enum\": [\n        \"active\",\n        \"closed\",\n        \"inactive\",\n        \"suspended\"\n      ],\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"description\": \"The time zone\
  \ of the balance account. For example, **Europe/Amsterdam**.\\nDefaults to the time zone of the account holder if no time zone is set. For possible values, see the [list of time zone codes](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderId\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-account-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceAccount
---
