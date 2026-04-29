---
description: Updates the number of pinned table header rows in a table.
layout: schema
name: PinTableHeaderRowsRequest
properties_list:
- description: The number of table rows to pin, where 0 implies that all rows are unpinned.
  name: pinnedHeaderRowsCount
  type: integer
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-pin-table-header-rows-request-schema.json
slug: google-docs-v1-pin-table-header-rows-request
source_filename: google-docs-v1-pin-table-header-rows-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PinTableHeaderRowsRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the number of pinned table header rows in a table.\",\n  \"properties\": {\n    \"pinnedHeaderRowsCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of table rows to pin, where 0 implies that all rows are unpinned.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-pin-table-header-rows-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: PinTableHeaderRowsRequest
---
