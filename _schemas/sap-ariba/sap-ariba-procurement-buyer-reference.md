---
description: Reference to a buyer organization
layout: schema
name: BuyerReference
properties_list:
- description: Buyer AN-ID on the SAP Ariba Network
  name: buyerId
  type: string
- description: Buyer organization name
  name: name
  type: string
- description: Buyer identifier in the ERP system
  name: erpBuyerId
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-buyer-reference-schema.json
slug: sap-ariba-procurement-buyer-reference
source_filename: sap-ariba-procurement-buyer-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuyerReference\",\n  \"type\": \"object\",\n  \"description\": \"Reference to a buyer organization\",\n  \"properties\": {\n    \"buyerId\": {\n      \"type\": \"string\",\n      \"description\": \"Buyer AN-ID on the SAP Ariba Network\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Buyer organization name\"\n    },\n    \"erpBuyerId\": {\n      \"type\": \"string\",\n      \"description\": \"Buyer identifier in the ERP system\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-buyer-reference-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: BuyerReference
---
