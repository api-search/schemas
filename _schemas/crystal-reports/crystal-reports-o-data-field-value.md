---
description: A single field value from an OData row
layout: schema
name: ODataFieldValue
properties_list:
- description: Name of the field
  name: fieldName
  type: string
- description: Value of the field
  name: value
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-o-data-field-value-schema.json
slug: crystal-reports-o-data-field-value
source_filename: crystal-reports-o-data-field-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-o-data-field-value-schema.json\",\n  \"title\": \"ODataFieldValue\",\n  \"description\": \"A single field value from an OData row\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the field\",\n      \"example\": \"CustomerName\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Value of the field\",\n      \"example\": \"City Cyclists\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-o-data-field-value-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: ODataFieldValue
---
