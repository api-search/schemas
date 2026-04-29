---
description: Postal address structure used for shipping, billing, and company addresses
layout: schema
name: Address
properties_list:
- description: Addressee name or attention line
  name: name
  type: string
- description: Street address lines
  name: lines
  type: string
- description: City name
  name: city
  type: string
- description: State or province
  name: state
  type: string
- description: Postal or ZIP code
  name: postalCode
  type: string
- description: Country code (ISO 3166-1 alpha-2)
  name: country
  type: string
- description: Phone number
  name: phone
  type: string
- description: Email address
  name: email
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-address-schema.json
slug: sap-ariba-procurement-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"description\": \"Postal address structure used for shipping, billing, and company addresses\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Addressee name or attention line\"\n    },\n    \"lines\": {\n      \"type\": \"string\",\n      \"description\": \"Street address lines\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (ISO 3166-1 alpha-2)\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number\"\n    },\n    \"email\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Email address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-address-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: Address
---
