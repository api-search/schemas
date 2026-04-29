---
description: AccountRegistration schema from Avalara API
layout: schema
name: AccountRegistration
properties_list:
- description: ''
  name: companyName
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: phoneNumber
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: partnerCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/business-account-registration-schema.json
slug: business-account-registration
source_filename: business-account-registration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/business-account-registration-schema.json\",\n  \"title\": \"AccountRegistration\",\n  \"description\": \"AccountRegistration schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"companyName\",\n    \"email\"\n  ],\n  \"properties\": {\n    \"companyName\": {\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"region\": {\n          \"\
  type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"partnerCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/business-account-registration-schema.json
tags:
- Taxes
title: AccountRegistration
---
