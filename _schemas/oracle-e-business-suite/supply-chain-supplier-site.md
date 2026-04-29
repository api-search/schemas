---
description: ''
layout: schema
name: SupplierSite
properties_list:
- description: Vendor site identifier
  name: vendorSiteId
  type: integer
- description: Vendor site code
  name: vendorSiteCode
  type: string
- description: ''
  name: addressLine1
  type: string
- description: ''
  name: addressLine2
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: zip
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: purchasingSiteFlag
  type: string
- description: ''
  name: paymentSiteFlag
  type: string
- description: ''
  name: orgId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-supplier-site-schema.json
slug: supply-chain-supplier-site
source_filename: supply-chain-supplier-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SupplierSite\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vendorSiteId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor site identifier\"\n    },\n    \"vendorSiteCode\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor site code\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"zip\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"purchasingSiteFlag\": {\n      \"type\": \"string\"\n    },\n    \"paymentSiteFlag\": {\n      \"type\": \"string\"\n    },\n    \"orgId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-supplier-site-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: SupplierSite
---
