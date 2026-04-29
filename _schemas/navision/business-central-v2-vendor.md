---
description: ''
layout: schema
name: Vendor
properties_list:
- description: ''
  name: '@odata.etag'
  type: string
- description: The unique identifier of the vendor
  name: id
  type: string
- description: The vendor number
  name: number
  type: string
- description: The vendor display name
  name: displayName
  type: string
- description: First line of the address
  name: addressLine1
  type: string
- description: Second line of the address
  name: addressLine2
  type: string
- description: The city
  name: city
  type: string
- description: The state or province code
  name: state
  type: string
- description: The country/region code
  name: country
  type: string
- description: The postal code
  name: postalCode
  type: string
- description: The phone number
  name: phoneNumber
  type: string
- description: The email address
  name: email
  type: string
- description: The website URL
  name: website
  type: string
- description: The tax registration number
  name: taxRegistrationNumber
  type: string
- description: The currency ID
  name: currencyId
  type: string
- description: The currency code
  name: currencyCode
  type: string
- description: The payment terms ID
  name: paymentTermsId
  type: string
- description: The payment method ID
  name: paymentMethodId
  type: string
- description: Whether the vendor is tax liable
  name: taxLiable
  type: boolean
- description: Whether the vendor is blocked
  name: blocked
  type: string
- description: The vendor balance
  name: balance
  type: number
- description: ''
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-vendor-schema.json
slug: business-central-v2-vendor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Vendor\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the vendor\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor number\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor display name\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of the address\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of the address\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province code\"\n    },\n    \"country\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"The country/region code\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"description\": \"The website URL\"\n    },\n    \"taxRegistrationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The tax registration number\"\n    },\n    \"currencyId\": {\n      \"type\": \"string\",\n      \"description\": \"The currency ID\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The currency code\"\n    },\n    \"paymentTermsId\": {\n      \"type\": \"string\",\n      \"description\": \"The payment terms ID\"\n    },\n    \"paymentMethodId\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The payment method ID\"\n    },\n    \"taxLiable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the vendor is tax liable\"\n    },\n    \"blocked\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the vendor is blocked\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"description\": \"The vendor balance\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-vendor-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Vendor
---
