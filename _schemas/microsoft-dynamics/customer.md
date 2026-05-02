---
description: A customer record in Microsoft Dynamics 365, representing a person or organization that purchases goods or services.
layout: schema
name: Customer
properties_list:
- description: The unique identifier of the customer.
  name: id
  type: string
- description: The customer number.
  name: number
  type: string
- description: The display name of the customer.
  name: displayName
  type: string
- description: The type of customer.
  name: type
  type: string
- description: The first line of the customer address.
  name: addressLine1
  type: string
- description: The second line of the customer address.
  name: addressLine2
  type: string
- description: The city of the customer address.
  name: city
  type: string
- description: The state or province of the customer address.
  name: state
  type: string
- description: The country or region of the customer address.
  name: country
  type: string
- description: The postal code of the customer address.
  name: postalCode
  type: string
- description: The phone number of the customer.
  name: phoneNumber
  type: string
- description: The email address of the customer.
  name: email
  type: string
- description: The website URL of the customer.
  name: website
  type: string
- description: The tax registration number.
  name: taxRegistrationNumber
  type: string
- description: The default currency code for the customer.
  name: currencyCode
  type: string
- description: Indicates whether the customer is blocked for transactions.
  name: blocked
  type: string
- description: The current balance of the customer.
  name: balance
  type: number
- description: The date and time the record was last modified.
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/customer.json
slug: customer
source_filename: customer.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/customer.json\",\n  \"title\": \"Customer\",\n  \"description\": \"A customer record in Microsoft Dynamics 365, representing a person or organization that purchases goods or services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the customer.\",\n      \"readOnly\": true\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The customer number.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the customer.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Person\", \"Company\"],\n      \"description\": \"The type of customer.\"\n    },\n    \"addressLine1\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The first line of the customer address.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"The second line of the customer address.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city of the customer address.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province of the customer address.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country or region of the customer address.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code of the customer address.\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the customer.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the customer.\"\
  \n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The website URL of the customer.\"\n    },\n    \"taxRegistrationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The tax registration number.\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The default currency code for the customer.\"\n    },\n    \"blocked\": {\n      \"type\": \"string\",\n      \"enum\": [\" \", \"Ship\", \"Invoice\", \"All\"],\n      \"description\": \"Indicates whether the customer is blocked for transactions.\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"description\": \"The current balance of the customer.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"\
  displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/customer.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Customer
---
