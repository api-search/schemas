---
description: CreateMerchantUserRequest schema from Adyen API
layout: schema
name: CreateMerchantUserRequest
properties_list:
- description: The list of [account groups](https://docs.adyen.com/account/account-structure#account-groups) associated with this user.
  name: accountGroups
  type: array
- description: The email address of the user.
  name: email
  type: string
- description: 'The user''s full name. Allowed length: 1—80 characters.'
  name: name
  type: object
- description: The list of [roles](https://docs.adyen.com/account/user-roles) for this user.
  name: roles
  type: array
- description: The [tz database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) of the time zone of the user. For example, **Europe/Amsterdam**.
  name: timeZoneCode
  type: string
- description: The user's email address that will be their username. Must be the same as the one in the `email` field.
  name: username
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-create-merchant-user-request-schema.json
slug: management-create-merchant-user-request
source_filename: management-create-merchant-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-merchant-user-request-schema.json\",\n  \"title\": \"CreateMerchantUserRequest\",\n  \"description\": \"CreateMerchantUserRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountGroups\": {\n      \"description\": \"The list of [account groups](https://docs.adyen.com/account/account-structure#account-groups) associated with this user.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"email\": {\n      \"description\": \"The email address of the user.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The user's full name.\\n\\nAllowed length: 1\\u201480 characters.\",\n      \"maxLength\": 80,\n      \"minLength\": 1,\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n\
  \    \"roles\": {\n      \"description\": \"The list of [roles](https://docs.adyen.com/account/user-roles) for this user.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"timeZoneCode\": {\n      \"description\": \"The [tz database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) of the time zone of the user. For example, **Europe/Amsterdam**.\",\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"description\": \"The user's email address that will be their username. Must be the same as the one in the `email` field.\",\n      \"maxLength\": 255,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"email\",\n    \"username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-merchant-user-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateMerchantUserRequest
---
