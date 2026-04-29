---
description: Deletes a NamedRange.
layout: schema
name: DeleteNamedRangeRequest
properties_list:
- description: The ID of the named range to delete.
  name: namedRangeId
  type: string
- description: The name of the range to delete. All named ranges with the given name will be deleted.
  name: name
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-delete-named-range-request-schema.json
slug: google-docs-v1-delete-named-range-request
source_filename: google-docs-v1-delete-named-range-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteNamedRangeRequest\",\n  \"type\": \"object\",\n  \"description\": \"Deletes a NamedRange.\",\n  \"properties\": {\n    \"namedRangeId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the named range to delete.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the range to delete. All named ranges with the given name will be deleted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-delete-named-range-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: DeleteNamedRangeRequest
---
