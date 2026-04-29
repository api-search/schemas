---
description: Represents a user's permission settings for a Google Tag Manager Account and its Containers.
layout: schema
name: UserPermission
properties_list:
- description: GTM UserPermission's API relative path.
  name: path
  type: string
- description: The Account ID uniquely identifies the GTM Account.
  name: accountId
  type: string
- description: User's email address.
  name: emailAddress
  type: string
- description: GTM Container access permissions.
  name: containerAccess
  type: array
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-user-permission-schema.json
slug: google-tag-manager-v2-user-permission
source_filename: google-tag-manager-v2-user-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserPermission\",\n  \"type\": \"object\",\n  \"description\": \"Represents a user's permission settings for a Google Tag Manager Account and its Containers.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"GTM UserPermission's API relative path.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The Account ID uniquely identifies the GTM Account.\"\n    },\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"description\": \"User's email address.\"\n    },\n    \"containerAccess\": {\n      \"type\": \"array\",\n      \"description\": \"GTM Container access permissions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-user-permission-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: UserPermission
---
