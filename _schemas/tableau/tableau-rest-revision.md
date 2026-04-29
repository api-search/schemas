---
description: ''
layout: schema
name: Revision
properties_list:
- description: The revision number.
  name: revisionNumber
  type: integer
- description: The date and time the revision was published.
  name: publishedAt
  type: string
- description: Whether this revision has been deleted.
  name: deleted
  type: boolean
- description: Whether this is the current revision.
  name: current
  type: boolean
- description: The size of the revision in bytes.
  name: sizeInBytes
  type: integer
- description: ''
  name: publisher
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-revision-schema.json
slug: tableau-rest-revision
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Revision\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"The revision number.\"\n    },\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the revision was published.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this revision has been deleted.\"\n    },\n    \"current\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the current revision.\"\n    },\n    \"sizeInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the revision in bytes.\"\n    },\n    \"publisher\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-revision-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Revision
---
