---
description: A vendor record in Microsoft Dynamics 365, representing a supplier of goods or services.
layout: schema
name: Vendor
properties_list:
- description: The unique identifier of the vendor.
  name: id
  type: string
- description: The vendor number.
  name: number
  type: string
- description: The display name of the vendor.
  name: displayName
  type: string
- description: The first line of the vendor address.
  name: addressLine1
  type: string
- description: The second line of the vendor address.
  name: addressLine2
  type: string
- description: The city of the vendor address.
  name: city
  type: string
- description: The state or province of the vendor address.
  name: state
  type: string
- description: The country or region of the vendor address.
  name: country
  type: string
- description: The postal code of the vendor address.
  name: postalCode
  type: string
- description: The phone number of the vendor.
  name: phoneNumber
  type: string
- description: The email address of the vendor.
  name: email
  type: string
- description: The website URL of the vendor.
  name: website
  type: string
- description: The tax registration number.
  name: taxRegistrationNumber
  type: string
- description: The default currency code for the vendor.
  name: currencyCode
  type: string
- description: The current balance owed to the vendor.
  name: balance
  type: number
- description: The date and time the record was last modified.
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/vendor.json
slug: vendor
source_filename: vendor.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/vendor.json\",\n  \"title\": \"Vendor\",\n  \"description\": \"A vendor record in Microsoft Dynamics 365, representing a supplier of goods or services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the vendor.\",\n      \"readOnly\": true\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor number.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the vendor.\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"The first line of the vendor address.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ second line of the vendor address.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city of the vendor address.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province of the vendor address.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country or region of the vendor address.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code of the vendor address.\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the vendor.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the vendor.\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The website URL of the vendor.\"\n    },\n    \"taxRegistrationNumber\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The tax registration number.\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The default currency code for the vendor.\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"description\": \"The current balance owed to the vendor.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/vendor.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Vendor
---
