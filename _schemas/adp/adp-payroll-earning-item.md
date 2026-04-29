---
description: ''
layout: schema
name: EarningItem
properties_list:
- description: ''
  name: typeCode
  type: object
- description: ''
  name: nameCode
  type: object
- description: ''
  name: hoursQuantity
  type: number
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-payroll-earning-item-schema.json
slug: adp-payroll-earning-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EarningItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"typeCode\": {\n      \"type\": \"object\"\n    },\n    \"nameCode\": {\n      \"type\": \"object\"\n    },\n    \"hoursQuantity\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-payroll-earning-item-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: EarningItem
---
