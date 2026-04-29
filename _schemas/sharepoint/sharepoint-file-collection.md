---
description: FileCollection from SharePoint API
layout: schema
name: FileCollection
properties_list:
- description: ''
  name: value
  type: array
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-file-collection-schema.json
slug: sharepoint-file-collection
source_filename: sharepoint-file-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-file-collection-schema.json\",\n  \"title\": \"FileCollection\",\n  \"description\": \"FileCollection from SharePoint API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/File\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-file-collection-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: FileCollection
---
