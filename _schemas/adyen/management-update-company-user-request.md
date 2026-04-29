---
description: UpdateCompanyUserRequest schema from Adyen API
layout: schema
name: UpdateCompanyUserRequest
properties_list:
- description: The list of [account groups](https://docs.adyen.com/account/account-structure#account-groups) associated with this user.
  name: accountGroups
  type: array
- description: Indicates whether this user is active.
  name: active
  type: boolean
- description: The list of [merchant accounts](https://docs.adyen.com/account/account-structure#merchant-accounts) to associate the user with.
  name: associatedMerchantAccounts
  type: array
- description: The email address of the user.
  name: email
  type: string
- description: The user's full name.
  name: name
  type: object
- description: The list of [roles](https://docs.adyen.com/account/user-roles) for this user.
  name: roles
  type: array
- description: The [tz database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) of the time zone of the user. For example, **Europe/Amsterdam**.
  name: timeZoneCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-update-company-user-request-schema.json
slug: management-update-company-user-request
source_filename: management-update-company-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-company-user-request-schema.json\",\n  \"title\": \"UpdateCompanyUserRequest\",\n  \"description\": \"UpdateCompanyUserRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountGroups\": {\n      \"description\": \"The list of [account groups](https://docs.adyen.com/account/account-structure#account-groups) associated with this user.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"active\": {\n      \"description\": \"Indicates whether this user is active.\",\n      \"type\": \"boolean\"\n    },\n    \"associatedMerchantAccounts\": {\n      \"description\": \"The list of [merchant accounts](https://docs.adyen.com/account/account-structure#merchant-accounts) to associate the user with.\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"email\": {\n      \"description\": \"The email address of the user.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The user's full name.\",\n      \"maxLength\": 80,\n      \"minLength\": 1,\n      \"$ref\": \"#/components/schemas/Name2\"\n    },\n    \"roles\": {\n      \"description\": \"The list of [roles](https://docs.adyen.com/account/user-roles) for this user.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"timeZoneCode\": {\n      \"description\": \"The [tz database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) of the time zone of the user. For example, **Europe/Amsterdam**.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-company-user-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateCompanyUserRequest
---
