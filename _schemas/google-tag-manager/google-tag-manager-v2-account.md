---
description: Represents a Google Tag Manager Account.
layout: schema
name: Account
properties_list:
- description: GTM Account's API relative path.
  name: path
  type: string
- description: The Account ID uniquely identifies the GTM Account.
  name: accountId
  type: string
- description: Account display name.
  name: name
  type: string
- description: Whether the account shares data anonymously with Google and others. This flag enables benchmarking by sharing your data in an anonymous form.
  name: shareData
  type: boolean
- description: The fingerprint of the GTM Account as computed at storage time. This value is recomputed whenever the account is modified.
  name: fingerprint
  type: string
- description: Auto-generated link to the tag manager UI.
  name: tagManagerUrl
  type: string
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-account-schema.json
slug: google-tag-manager-v2-account
source_filename: google-tag-manager-v2-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Google Tag Manager Account.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Account's API relative path.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The Account ID uniquely identifies the GTM Account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Account display name.\"\n    },\n    \"shareData\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account shares data anonymously with Google and others. This flag enables benchmarking by sharing your data in an anonymous form.\"\n    },\n    \"fingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"The fingerprint of the GTM Account as computed at storage time. This value is recomputed whenever the account is modified.\"\
  \n    },\n    \"tagManagerUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated link to the tag manager UI.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-account-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: Account
---
