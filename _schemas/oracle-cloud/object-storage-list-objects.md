---
description: Response containing a list of objects.
layout: schema
name: ListObjects
properties_list:
- description: List of object summaries.
  name: objects
  type: array
- description: Prefixes for pseudo-directory grouping.
  name: prefixes
  type: array
- description: Object name to resume listing.
  name: nextStartWith
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/object-storage-list-objects-schema.json
slug: object-storage-list-objects
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-list-objects-schema.json\",\n  \"title\": \"ListObjects\",\n  \"description\": \"Response containing a list of objects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"objects\": {\n      \"type\": \"array\",\n      \"description\": \"List of object summaries.\",\n      \"example\": \"[{'name': 'documents/report.pdf', 'size': 1048576, 'md5': 'aGVsbG93b3JsZA==', 'timeCreated': '2026-04-18T10:30:00Z', 'timeModified': '2026-04-18T10:30:00Z', 'storageTier': 'Standard'}]\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"prefixes\": {\n      \"type\": \"array\",\n      \"description\": \"Prefixes for pseudo-directory grouping.\",\n      \"example\": \"['example-value']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"nextStartWith\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Object name to resume listing.\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-list-objects-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: ListObjects
---
