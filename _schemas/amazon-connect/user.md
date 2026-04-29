---
description: Contains information about a user account for an Amazon Connect instance.
layout: schema
name: User
properties_list:
- description: The identifier of the user account.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the user account.
  name: Arn
  type: string
- description: The user name assigned to the user account.
  name: Username
  type: string
- description: ''
  name: IdentityInfo
  type: object
- description: ''
  name: PhoneConfig
  type: object
- description: The identifier of the user account in the directory service that Amazon Connect uses to authenticate users.
  name: DirectoryUserId
  type: string
- description: The identifiers of the security profiles for the user.
  name: SecurityProfileIds
  type: array
- description: The identifier of the routing profile for the user.
  name: RoutingProfileId
  type: string
- description: The identifier of the hierarchy group for the user.
  name: HierarchyGroupId
  type: string
- description: The tags.
  name: Tags
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/user-schema.json
slug: user
source_filename: user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"Contains information about a user account for an Amazon Connect instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user account.\",\n      \"example\": \"500123\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the user account.\",\n      \"example\": \"arn:aws:connect:us-east-1:123456789012:instance/a1b2c3d4/agent/500123\"\n    },\n    \"Username\": {\n      \"type\": \"string\",\n      \"description\": \"The user name assigned to the user account.\",\n      \"example\": \"jsmith\"\n    },\n    \"IdentityInfo\": {\n      \"$ref\": \"#/components/schemas/UserIdentityInfo\"\n \
  \   },\n    \"PhoneConfig\": {\n      \"$ref\": \"#/components/schemas/UserPhoneConfig\"\n    },\n    \"DirectoryUserId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user account in the directory service that Amazon Connect uses to authenticate users.\"\n    },\n    \"SecurityProfileIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The identifiers of the security profiles for the user.\"\n    },\n    \"RoutingProfileId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the routing profile for the user.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-33333EXAMPLE\"\n    },\n    \"HierarchyGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the hierarchy group for the user.\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"The tags.\",\n      \"additionalProperties\": {\n        \"type\"\
  : \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/user-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: User
---
