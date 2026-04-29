---
description: Physical (mailing) address
layout: schema
name: PhysicalAddress
properties_list:
- description: Unique identifier for the address
  name: Id
  type: string
- description: First line of the street address
  name: Line1
  type: string
- description: Second line of the street address
  name: Line2
  type: string
- description: Third line of the street address
  name: Line3
  type: string
- description: Fourth line of the street address
  name: Line4
  type: string
- description: Fifth line of the street address
  name: Line5
  type: string
- description: City name
  name: City
  type: string
- description: Region or state within a country (e.g., state, province)
  name: CountrySubDivisionCode
  type: string
- description: Postal code
  name: PostalCode
  type: string
- description: Country name or code
  name: Country
  type: string
- description: Latitude coordinate
  name: Lat
  type: string
- description: Longitude coordinate
  name: Long
  type: string
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-physical-address-schema.json
slug: quickbooks-accounting-physical-address
source_filename: quickbooks-accounting-physical-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PhysicalAddress\",\n  \"type\": \"object\",\n  \"description\": \"Physical (mailing) address\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the address\"\n    },\n    \"Line1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of the street address\"\n    },\n    \"Line2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of the street address\"\n    },\n    \"Line3\": {\n      \"type\": \"string\",\n      \"description\": \"Third line of the street address\"\n    },\n    \"Line4\": {\n      \"type\": \"string\",\n      \"description\": \"Fourth line of the street address\"\n    },\n    \"Line5\": {\n      \"type\": \"string\",\n      \"description\": \"Fifth line of the street address\"\n    },\n    \"City\": {\n      \"type\": \"string\",\n      \"description\": \"City name\"\n    },\n\
  \    \"CountrySubDivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Region or state within a country (e.g., state, province)\"\n    },\n    \"PostalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code\"\n    },\n    \"Country\": {\n      \"type\": \"string\",\n      \"description\": \"Country name or code\"\n    },\n    \"Lat\": {\n      \"type\": \"string\",\n      \"description\": \"Latitude coordinate\"\n    },\n    \"Long\": {\n      \"type\": \"string\",\n      \"description\": \"Longitude coordinate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-physical-address-schema.json
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
title: PhysicalAddress
---
