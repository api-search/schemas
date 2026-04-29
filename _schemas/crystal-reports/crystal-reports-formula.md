---
description: A formula field defined in the report
layout: schema
name: Formula
properties_list:
- description: Formula field name
  name: name
  type: string
- description: Formula expression text
  name: text
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-formula-schema.json
slug: crystal-reports-formula
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-formula-schema.json\",\n  \"title\": \"Formula\",\n  \"description\": \"A formula field defined in the report\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Formula field name\",\n      \"example\": \"FullAddress\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Formula expression text\",\n      \"example\": \"{Customer.Address1} & \\\", \\\" & {Customer.City}\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-formula-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: Formula
---
