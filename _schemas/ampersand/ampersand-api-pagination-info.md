---
description: PaginationInfo schema from Ampersand API
layout: schema
name: PaginationInfo
properties_list:
- description: If set to true, this is the last page of results for the given operation. There are no more results & there will be no nextPageToken sent when done is true.
  name: done
  type: boolean
- description: If present, set this value against your 'pageToken' query parameter in the next API call, which will retrieve the next set of results.
  name: nextPageToken
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-pagination-info-schema.json
slug: ampersand-api-pagination-info
source_filename: ampersand-api-pagination-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-pagination-info-schema.json\",\n  \"title\": \"PaginationInfo\",\n  \"description\": \"PaginationInfo schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"done\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, this is the last page of results for the given operation. There are no more results & there will be no nextPageToken sent when done is true.\",\n      \"example\": false\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"If present, set this value against your 'pageToken' query parameter in the next API call, which will retrieve the next set of results.\",\n      \"example\": \"Q9JT+2qfys28V4ODN+UayA==\"\n    }\n  },\n  \"required\": [\n    \"done\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-pagination-info-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: PaginationInfo
---
