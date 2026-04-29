---
description: ''
layout: schema
name: GetLibraryAnalyticsUsagesResponseBody
properties_list:
- description: An array of analytics data when breaking down usage by component.
  name: components
  type: array
- description: An array of analytics data when breaking down usage by file.
  name: files
  type: array
- description: Whether there is a next page of data that can be fetched.
  name: nextPage
  type: boolean
- description: The cursor to use to fetch the next page of data. Not present if nextPage is false.
  name: cursor
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-analytics-get-library-analytics-usages-response-body-schema.json
slug: figma-analytics-get-library-analytics-usages-response-body
source_filename: figma-analytics-get-library-analytics-usages-response-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetLibraryAnalyticsUsagesResponseBody\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"components\": {\n      \"type\": \"array\",\n      \"description\": \"An array of analytics data when breaking down usage by component.\"\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"An array of analytics data when breaking down usage by file.\"\n    },\n    \"nextPage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there is a next page of data that can be fetched.\"\n    },\n    \"cursor\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor to use to fetch the next page of data. Not present if nextPage is false.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-analytics-get-library-analytics-usages-response-body-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetLibraryAnalyticsUsagesResponseBody
---
