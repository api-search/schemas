---
description: Represents a customer entity in Dynamics 365 Business Central. Customers are the parties to whom the company sells goods or services. Each customer record contains contact information, financial settings, and trading terms.
layout: schema
name: Customer
properties_list:
- description: ETag for optimistic concurrency control
  name: '@odata.etag'
  type: string
- description: The unique identifier (GUID) of the customer record
  name: id
  type: string
- description: The customer number, a unique business identifier assigned automatically or manually
  name: number
  type: string
- description: The display name of the customer (individual or company name)
  name: displayName
  type: string
- description: Specifies whether the customer is an individual person or a company
  name: type
  type: string
- description: The first line of the customer's street address
  name: addressLine1
  type: string
- description: The second line of the customer's street address
  name: addressLine2
  type: string
- description: The city of the customer's address
  name: city
  type: string
- description: The state or province code of the customer's address
  name: state
  type: string
- description: The country/region code of the customer's address
  name: country
  type: string
- description: The postal or ZIP code of the customer's address
  name: postalCode
  type: string
- description: The customer's primary phone number
  name: phoneNumber
  type: string
- description: The customer's email address
  name: email
  type: string
- description: The customer's website URL
  name: website
  type: string
- description: The code of the salesperson assigned to this customer
  name: salespersonCode
  type: string
- description: The total balance due from the customer (read-only, computed)
  name: balanceDue
  type: number
- description: The maximum credit amount allowed for the customer
  name: creditLimit
  type: number
- description: Indicates whether the customer is liable for sales tax
  name: taxLiable
  type: boolean
- description: The unique identifier of the tax area assigned to the customer
  name: taxAreaId
  type: string
- description: The display name of the tax area (read-only)
  name: taxAreaDisplayName
  type: string
- description: The customer's tax registration number (VAT number or similar)
  name: taxRegistrationNumber
  type: string
- description: The unique identifier of the currency used for this customer
  name: currencyId
  type: string
- description: The currency code (e.g., USD, EUR) used for transactions with this customer
  name: currencyCode
  type: string
- description: The unique identifier of the payment terms assigned to the customer
  name: paymentTermsId
  type: string
- description: The unique identifier of the shipment method
  name: shipmentMethodId
  type: string
- description: The unique identifier of the payment method
  name: paymentMethodId
  type: string
- description: 'Specifies which transactions are blocked for the customer: blank (none), Ship, Invoice, or All'
  name: blocked
  type: string
- description: The date and time the customer record was last modified (read-only)
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/customer.json
slug: customer
source_filename: customer.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://example.com/schemas/navision/customer.json\",\n  \"title\": \"Customer\",\n  \"description\": \"Represents a customer entity in Dynamics 365 Business Central. Customers are the parties to whom the company sells goods or services. Each customer record contains contact information, financial settings, and trading terms.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for optimistic concurrency control\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier (GUID) of the customer record\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The customer number, a unique business identifier assigned automatically or manually\"\n    },\n    \"displayName\": {\n      \"type\": \"\
  string\",\n      \"maxLength\": 100,\n      \"description\": \"The display name of the customer (individual or company name)\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Person\", \"Company\"],\n      \"description\": \"Specifies whether the customer is an individual person or a company\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The first line of the customer's street address\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"The second line of the customer's street address\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"maxLength\": 30,\n      \"description\": \"The city of the customer's address\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The state or province code of the customer's address\"\n    },\n    \"country\": {\n      \"type\"\
  : \"string\",\n      \"maxLength\": 10,\n      \"description\": \"The country/region code of the customer's address\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The postal or ZIP code of the customer's address\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"maxLength\": 30,\n      \"description\": \"The customer's primary phone number\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"maxLength\": 80,\n      \"format\": \"email\",\n      \"description\": \"The customer's email address\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"maxLength\": 80,\n      \"format\": \"uri\",\n      \"description\": \"The customer's website URL\"\n    },\n    \"salespersonCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The code of the salesperson assigned to this customer\"\n    },\n    \"balanceDue\": {\n      \"type\": \"number\",\n\
  \      \"description\": \"The total balance due from the customer (read-only, computed)\",\n      \"readOnly\": true\n    },\n    \"creditLimit\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum credit amount allowed for the customer\"\n    },\n    \"taxLiable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the customer is liable for sales tax\"\n    },\n    \"taxAreaId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the tax area assigned to the customer\"\n    },\n    \"taxAreaDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the tax area (read-only)\",\n      \"readOnly\": true\n    },\n    \"taxRegistrationNumber\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"The customer's tax registration number (VAT number or similar)\"\n    },\n    \"currencyId\": {\n      \"type\": \"string\",\n   \
  \   \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the currency used for this customer\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"The currency code (e.g., USD, EUR) used for transactions with this customer\"\n    },\n    \"paymentTermsId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the payment terms assigned to the customer\"\n    },\n    \"shipmentMethodId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the shipment method\"\n    },\n    \"paymentMethodId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the payment method\"\n    },\n    \"blocked\": {\n      \"type\": \"string\",\n      \"enum\": [\" \", \"Ship\", \"Invoice\", \"All\"],\n      \"description\": \"Specifies which transactions\
  \ are blocked for the customer: blank (none), Ship, Invoice, or All\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the customer record was last modified (read-only)\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"id\", \"displayName\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/customer.json
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
