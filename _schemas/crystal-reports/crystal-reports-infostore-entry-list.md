---
description: A collection of infostore entries
layout: schema
name: InfostoreEntryList
properties_list:
- description: List of infostore objects
  name: entries
  type: array
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-infostore-entry-list-schema.json
slug: crystal-reports-infostore-entry-list
source_filename: crystal-reports-infostore-entry-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-infostore-entry-list-schema.json\",\n  \"title\": \"InfostoreEntryList\",\n  \"description\": \"A collection of infostore entries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entries\": {\n      \"type\": \"array\",\n      \"description\": \"List of infostore objects\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InfostoreEntry\"\n      },\n      \"example\": [\n        {\n          \"id\": 4201,\n          \"cuid\": \"AaGKDkx9w5RMoGANrfKwmn0\",\n          \"name\": \"Report Samples\",\n          \"type\": \"Folder\",\n          \"description\": \"Sample Crystal Reports\",\n          \"uri\": \"/biprws/infostore/4201\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-infostore-entry-list-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: InfostoreEntryList
---
