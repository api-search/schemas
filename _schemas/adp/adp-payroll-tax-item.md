---
description: ''
layout: schema
name: TaxItem
properties_list:
- description: ''
  name: typeCode
  type: object
- description: ''
  name: nameCode
  type: object
- description: ''
  name: jurisdictionCode
  type: object
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-payroll-tax-item-schema.json
slug: adp-payroll-tax-item
source_filename: adp-payroll-tax-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaxItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"typeCode\": {\n      \"type\": \"object\"\n    },\n    \"nameCode\": {\n      \"type\": \"object\"\n    },\n    \"jurisdictionCode\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-payroll-tax-item-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: TaxItem
---
