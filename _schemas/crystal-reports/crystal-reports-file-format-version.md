---
description: Crystal Report file format version
layout: schema
name: FileFormatVersion
properties_list:
- description: Major version number
  name: major_version
  type: integer
- description: Minor version number
  name: minor_version
  type: integer
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-file-format-version-schema.json
slug: crystal-reports-file-format-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-file-format-version-schema.json\",\n  \"title\": \"FileFormatVersion\",\n  \"description\": \"Crystal Report file format version\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"major_version\": {\n      \"type\": \"integer\",\n      \"description\": \"Major version number\",\n      \"example\": 14\n    },\n    \"minor_version\": {\n      \"type\": \"integer\",\n      \"description\": \"Minor version number\",\n      \"example\": 3\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-file-format-version-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: FileFormatVersion
---
