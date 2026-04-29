---
description: UNSPSC commodity classification code
layout: schema
name: CommodityCode
properties_list:
- description: UNSPSC commodity code
  name: code
  type: string
- description: Commodity description
  name: description
  type: string
- description: Classification domain identifier
  name: domain
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-commodity-code-schema.json
slug: sap-ariba-procurement-commodity-code
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommodityCode\",\n  \"type\": \"object\",\n  \"description\": \"UNSPSC commodity classification code\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"UNSPSC commodity code\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity description\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Classification domain identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-commodity-code-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: CommodityCode
---
