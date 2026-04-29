---
description: Contact information for a person or department
layout: schema
name: ContactInfo
properties_list:
- description: Contact person name
  name: name
  type: string
- description: Contact email address
  name: email
  type: string
- description: Contact phone number
  name: phone
  type: string
- description: Contact fax number
  name: fax
  type: string
- description: Department name
  name: department
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-contact-info-schema.json
slug: sap-ariba-procurement-contact-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactInfo\",\n  \"type\": \"object\",\n  \"description\": \"Contact information for a person or department\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact person name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Contact email address\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Contact phone number\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"description\": \"Contact fax number\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-contact-info-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: ContactInfo
---
