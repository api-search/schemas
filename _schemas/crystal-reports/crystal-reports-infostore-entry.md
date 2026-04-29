---
description: An object in the infostore repository (folder, report, etc.)
layout: schema
name: InfostoreEntry
properties_list:
- description: Unique infostore object identifier
  name: id
  type: integer
- description: Cluster unique identifier
  name: cuid
  type: string
- description: Display name of the object
  name: name
  type: string
- description: Object type (e.g., Folder, CrystalReport)
  name: type
  type: string
- description: Object description
  name: description
  type: string
- description: Relative URI to access this object
  name: uri
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-infostore-entry-schema.json
slug: crystal-reports-infostore-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-infostore-entry-schema.json\",\n  \"title\": \"InfostoreEntry\",\n  \"description\": \"An object in the infostore repository (folder, report, etc.)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique infostore object identifier\",\n      \"example\": 5765\n    },\n    \"cuid\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster unique identifier\",\n      \"example\": \"AaGKDkx9w5RMoGANrfKwmn0\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the object\",\n      \"example\": \"Sales Report Q4\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Object type (e.g., Folder, CrystalReport)\",\n      \"example\": \"CrystalReport\"\
  \n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Object description\",\n      \"example\": \"Quarterly sales report for all regions\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URI to access this object\",\n      \"example\": \"/biprws/infostore/5765\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-infostore-entry-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: InfostoreEntry
---
