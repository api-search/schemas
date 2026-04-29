---
description: BalanceAccountUpdateRequest schema from Adyen API
layout: schema
name: BalanceAccountUpdateRequest
properties_list:
- description: The unique identifier of the [account holder](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/accountHolders__resParam_id) associated with the balance account.
  name: accountHolderId
  type: string
- description: A human-readable description of the balance account, maximum 300 characters. You can use this parameter to distinguish between multiple balance accounts under an account holder.
  name: description
  type: string
- description: A set of key and value pairs for general use. The keys do not have specific names and may be used for storing miscellaneous data as desired. > Note that during an update of metadata, the omission of e
  name: metadata
  type: object
- description: Contains key-value pairs to the configure the settlement model in a balance account.
  name: platformPaymentConfiguration
  type: object
- description: Your reference to the balance account, maximum 150 characters.
  name: reference
  type: string
- description: 'The status of the balance account. Payment instruments linked to the balance account can only be used if the balance account status is **active**. Possible values: **active**, **inactive**, **closed**'
  name: status
  type: string
- description: The time zone of the balance account. For example, **Europe/Amsterdam**. Defaults to the time zone of the account holder if no time zone is set. For possible values, see the [list of time zone codes](
  name: timeZone
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-balance-account-update-request-schema.json
slug: configuration-balance-account-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-account-update-request-schema.json\",\n  \"title\": \"BalanceAccountUpdateRequest\",\n  \"description\": \"BalanceAccountUpdateRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderId\": {\n      \"description\": \"The unique identifier of the [account holder](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/accountHolders__resParam_id) associated with the balance account.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"A human-readable description of the balance account, maximum 300 characters. You can use this parameter to distinguish between multiple balance accounts under an account holder.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"\
  additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of key and value pairs for general use.\\nThe keys do not have specific names and may be used for storing miscellaneous data as desired.\\n> Note that during an update of metadata, the omission of existing key-value pairs will result in the deletion of those key-value pairs.\",\n      \"type\": \"object\"\n    },\n    \"platformPaymentConfiguration\": {\n      \"description\": \"Contains key-value pairs to the configure the settlement model in a balance account.\",\n      \"$ref\": \"#/components/schemas/PlatformPaymentConfiguration\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference to the balance account, maximum 150 characters.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the balance account. Payment instruments linked to the balance account can only be used if the balance account status\
  \ is **active**.\\n\\nPossible values: **active**, **inactive**, **closed**, **suspended**.\",\n      \"enum\": [\n        \"active\",\n        \"closed\",\n        \"inactive\",\n        \"suspended\"\n      ],\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"description\": \"The time zone of the balance account. For example, **Europe/Amsterdam**.\\nDefaults to the time zone of the account holder if no time zone is set. For possible values, see the [list of time zone codes](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-account-update-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceAccountUpdateRequest
---
