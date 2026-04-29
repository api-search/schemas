---
description: Schema for a Hugging Face user account including profile information, organizations, and subscription details.
layout: schema
name: Hugging Face User
properties_list:
- description: Account type
  name: type
  type: string
- description: Unique user identifier
  name: id
  type: string
- description: Username (handle)
  name: name
  type: string
- description: Full display name
  name: fullname
  type: string
- description: Email address
  name: email
  type: string
- description: Whether the email has been verified
  name: emailVerified
  type: boolean
- description: Subscription plan
  name: plan
  type: string
- description: Whether the user is on a Pro plan
  name: isPro
  type: boolean
- description: Whether the user has a payment method configured
  name: canPay
  type: boolean
- description: URL to the user's avatar image
  name: avatarUrl
  type: string
- description: Organizations the user belongs to
  name: orgs
  type: array
- description: Authentication information
  name: auth
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-user-schema.json
slug: hugging-face-user
source_filename: hugging-face-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://huggingface.co/schemas/user.json\",\n  \"title\": \"Hugging Face User\",\n  \"description\": \"Schema for a Hugging Face user account including profile information, organizations, and subscription details.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Account type\",\n      \"enum\": [\n        \"user\",\n        \"org\"\n      ]\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Username (handle)\",\n      \"examples\": [\n        \"julien-c\",\n        \"lysandre\"\n      ]\n    },\n    \"fullname\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"email\",\n      \"description\": \"Email address\"\n    },\n    \"emailVerified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email has been verified\"\n    },\n    \"plan\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription plan\",\n      \"enum\": [\n        \"free\",\n        \"pro\",\n        \"enterprise\"\n      ]\n    },\n    \"isPro\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is on a Pro plan\"\n    },\n    \"canPay\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has a payment method configured\"\n    },\n    \"avatarUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the user's avatar image\"\n    },\n    \"orgs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Organization\
  \ username\"\n          },\n          \"fullname\": {\n            \"type\": \"string\",\n            \"description\": \"Organization display name\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          },\n          \"plan\": {\n            \"type\": \"string\"\n          },\n          \"avatarUrl\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"isEnterprise\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this is an Enterprise organization\"\n          },\n          \"periodEnd\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Subscription period end date\"\n          },\n          \"role\": {\n            \"type\": \"string\",\n            \"description\": \"User's role in this organization\",\n            \"enum\": [\n              \"admin\",\n              \"write\",\n     \
  \         \"read\",\n              \"contributor\"\n            ]\n          }\n        }\n      },\n      \"description\": \"Organizations the user belongs to\"\n    },\n    \"auth\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication information\",\n      \"properties\": {\n        \"accessToken\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"displayName\": {\n              \"type\": \"string\",\n              \"description\": \"Token display name\"\n            },\n            \"role\": {\n              \"type\": \"string\",\n              \"description\": \"Token role/permissions\"\n            },\n            \"createdAt\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-user-schema.json
tags: []
title: Hugging Face User
---
