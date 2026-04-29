---
description: CreateUserRequest schema from Amazon Connect Service API
layout: schema
name: CreateUserRequest
properties_list:
- description: The user name for the account.
  name: Username
  type: string
- description: The password for the user account.
  name: Password
  type: string
- description: ''
  name: IdentityInfo
  type: object
- description: ''
  name: PhoneConfig
  type: object
- description: ''
  name: DirectoryUserId
  type: string
- description: The identifier of the security profile for the user.
  name: SecurityProfileIds
  type: array
- description: The identifier of the routing profile for the user.
  name: RoutingProfileId
  type: string
- description: ''
  name: HierarchyGroupId
  type: string
- description: ''
  name: Tags
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-user-request-schema.json
slug: create-user-request
source_filename: create-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-user-request-schema.json\",\n  \"title\": \"CreateUserRequest\",\n  \"description\": \"CreateUserRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Username\": {\n      \"type\": \"string\",\n      \"description\": \"The user name for the account.\",\n      \"example\": \"jsmith\"\n    },\n    \"Password\": {\n      \"type\": \"string\",\n      \"description\": \"The password for the user account.\"\n    },\n    \"IdentityInfo\": {\n      \"$ref\": \"#/components/schemas/UserIdentityInfo\"\n    },\n    \"PhoneConfig\": {\n      \"$ref\": \"#/components/schemas/UserPhoneConfig\"\n    },\n    \"DirectoryUserId\": {\n      \"type\": \"string\"\n    },\n    \"SecurityProfileIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\":\
  \ \"string\"\n      },\n      \"description\": \"The identifier of the security profile for the user.\"\n    },\n    \"RoutingProfileId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the routing profile for the user.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-33333EXAMPLE\"\n    },\n    \"HierarchyGroupId\": {\n      \"type\": \"string\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"PhoneConfig\",\n    \"RoutingProfileId\",\n    \"SecurityProfileIds\",\n    \"Username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-user-request-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateUserRequest
---
