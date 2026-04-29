---
description: ''
layout: schema
name: Customer
properties_list:
- description: ETag for concurrency control
  name: '@odata.etag'
  type: string
- description: The unique identifier of the customer
  name: id
  type: string
- description: The customer number
  name: number
  type: string
- description: The customer display name
  name: displayName
  type: string
- description: The customer type
  name: type
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
- description: The salesperson code
  name: salespersonCode
  type: string
- description: The balance due from the customer
  name: balanceDue
  type: number
- description: The credit limit
  name: creditLimit
  type: number
- description: Whether the customer is tax liable
  name: taxLiable
  type: boolean
- description: The tax area ID
  name: taxAreaId
  type: string
- description: The tax area display name
  name: taxAreaDisplayName
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
- description: The shipment method ID
  name: shipmentMethodId
  type: string
- description: The payment method ID
  name: paymentMethodId
  type: string
- description: Whether the customer is blocked
  name: blocked
  type: string
- description: The date and time when the customer was last modified
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-customer-schema.json
slug: business-central-v2-customer
source_filename: business-central-v2-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Customer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for concurrency control\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the customer\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The customer number\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The customer display name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The customer type\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of the address\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of the address\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The city\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country/region code\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"description\": \"The website URL\"\n    },\n    \"salespersonCode\": {\n      \"type\": \"string\",\n      \"description\": \"The salesperson code\"\n    },\n    \"balanceDue\": {\n      \"type\": \"number\",\n      \"description\": \"The balance due from the customer\"\n    },\n    \"creditLimit\": {\n      \"type\": \"number\",\n      \"description\": \"The credit limit\"\n    },\n  \
  \  \"taxLiable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer is tax liable\"\n    },\n    \"taxAreaId\": {\n      \"type\": \"string\",\n      \"description\": \"The tax area ID\"\n    },\n    \"taxAreaDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The tax area display name\"\n    },\n    \"taxRegistrationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The tax registration number\"\n    },\n    \"currencyId\": {\n      \"type\": \"string\",\n      \"description\": \"The currency ID\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The currency code\"\n    },\n    \"paymentTermsId\": {\n      \"type\": \"string\",\n      \"description\": \"The payment terms ID\"\n    },\n    \"shipmentMethodId\": {\n      \"type\": \"string\",\n      \"description\": \"The shipment method ID\"\n    },\n    \"paymentMethodId\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ payment method ID\"\n    },\n    \"blocked\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the customer is blocked\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the customer was last modified\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-customer-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: Customer
---
