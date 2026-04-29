---
description: Unit of measure specification following UN/ECE Recommendation 20 standard codes
layout: schema
name: UnitOfMeasure
properties_list:
- description: Unit of measure code (UN/ECE Rec 20 or SAP Ariba internal code)
  name: code
  type: string
- description: Human-readable description of the unit
  name: description
  type: string
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-unit-of-measure-schema.json
slug: sap-ariba-procurement-unit-of-measure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UnitOfMeasure\",\n  \"type\": \"object\",\n  \"description\": \"Unit of measure specification following UN/ECE Recommendation 20 standard codes\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure code (UN/ECE Rec 20 or SAP Ariba internal code)\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the unit\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-unit-of-measure-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: UnitOfMeasure
---
