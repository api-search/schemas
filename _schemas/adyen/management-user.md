---
description: User schema from Adyen API
layout: schema
name: User
properties_list:
- description: References to resources connected with this user.
  name: _links
  type: object
- description: The list of [account groups](https://docs.adyen.com/account/account-structure#account-groups) associated with this user.
  name: accountGroups
  type: array
- description: Indicates whether this user is active.
  name: active
  type: boolean
- description: Set of apps available to this user
  name: apps
  type: array
- description: The email address of the user.
  name: email
  type: string
- description: The unique identifier of the user.
  name: id
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
- description: The username for this user.
  name: username
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-user-schema.json
slug: management-user
source_filename: management-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"User schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"description\": \"References to resources connected with this user.\",\n      \"$ref\": \"#/components/schemas/Links\"\n    },\n    \"accountGroups\": {\n      \"description\": \"The list of [account groups](https://docs.adyen.com/account/account-structure#account-groups) associated with this user.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"active\": {\n      \"description\": \"Indicates whether this user is active.\",\n      \"type\": \"boolean\"\n    },\n    \"apps\": {\n      \"description\": \"Set of apps available to this user\",\n      \"items\": {\n        \"type\": \"\
  string\"\n      },\n      \"type\": \"array\"\n    },\n    \"email\": {\n      \"description\": \"The email address of the user.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the user.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The user's full name.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"roles\": {\n      \"description\": \"The list of [roles](https://docs.adyen.com/account/user-roles) for this user.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"timeZoneCode\": {\n      \"description\": \"The [tz database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) of the time zone of the user. For example, **Europe/Amsterdam**.\",\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"description\": \"The username for this user.\",\n      \"maxLength\": 255,\n      \"minLength\": 1,\n  \
  \    \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"email\",\n    \"timeZoneCode\",\n    \"username\",\n    \"roles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-user-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: User
---
