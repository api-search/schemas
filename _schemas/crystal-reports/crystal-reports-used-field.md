---
description: A field used in the report
layout: schema
name: UsedField
properties_list:
- description: Field name
  name: name
  type: string
- description: Table the field belongs to
  name: table
  type: string
- description: Data type of the field
  name: type
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-used-field-schema.json
slug: crystal-reports-used-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-used-field-schema.json\",\n  \"title\": \"UsedField\",\n  \"description\": \"A field used in the report\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Field name\",\n      \"example\": \"Customer Name\"\n    },\n    \"table\": {\n      \"type\": \"string\",\n      \"description\": \"Table the field belongs to\",\n      \"example\": \"Customer\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the field\",\n      \"example\": \"String\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-used-field-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: UsedField
---
