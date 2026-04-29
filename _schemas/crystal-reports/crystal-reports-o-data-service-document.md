---
description: OData service document listing available collections
layout: schema
name: ODataServiceDocument
properties_list:
- description: Available entity set collections
  name: EntitySets
  type: array
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-o-data-service-document-schema.json
slug: crystal-reports-o-data-service-document
source_filename: crystal-reports-o-data-service-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-o-data-service-document-schema.json\",\n  \"title\": \"ODataServiceDocument\",\n  \"description\": \"OData service document listing available collections\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntitySets\": {\n      \"type\": \"array\",\n      \"description\": \"Available entity set collections\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"Rows\",\n        \"GrandTotals\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-o-data-service-document-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: ODataServiceDocument
---
