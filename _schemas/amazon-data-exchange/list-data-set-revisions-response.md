---
description: Response containing a list of revisions.
layout: schema
name: List Data Set Revisions Response
properties_list:
- description: ''
  name: Revisions
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/list-data-set-revisions-response-schema.json
slug: list-data-set-revisions-response
source_filename: list-data-set-revisions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/list-data-set-revisions-response-schema.json\",\n  \"title\": \"List Data Set Revisions Response\",\n  \"description\": \"Response containing a list of revisions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Revisions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"revision-schema.json\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/list-data-set-revisions-response-schema.json
tags:
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: List Data Set Revisions Response
---
