---
description: Response containing a list of DataZone domains.
layout: schema
name: List Domains Response
properties_list:
- description: ''
  name: items
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/list-domains-response-schema.json
slug: list-domains-response
source_filename: list-domains-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/list-domains-response-schema.json\",\n  \"title\": \"List Domains Response\",\n  \"description\": \"Response containing a list of DataZone domains.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/list-domains-response-schema.json
tags:
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: List Domains Response
---
