---
description: Library analytics actions data broken down by component.
layout: schema
name: LibraryAnalyticsActionsByComponent
properties_list:
- description: The date in ISO 8601 format. e.g. 2023-12-13
  name: week
  type: string
- description: Unique, stable id of the component.
  name: componentKey
  type: string
- description: Name of the component.
  name: componentName
  type: string
- description: The number of detach events for this period.
  name: detachments
  type: number
- description: The number of insertion events for this period.
  name: insertions
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-analytics-library-analytics-actions-by-component-schema.json
slug: figma-analytics-library-analytics-actions-by-component
source_filename: figma-analytics-library-analytics-actions-by-component-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryAnalyticsActionsByComponent\",\n  \"type\": \"object\",\n  \"description\": \"Library analytics actions data broken down by component.\",\n  \"properties\": {\n    \"week\": {\n      \"type\": \"string\",\n      \"description\": \"The date in ISO 8601 format. e.g. 2023-12-13\"\n    },\n    \"componentKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique, stable id of the component.\"\n    },\n    \"componentName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the component.\"\n    },\n    \"detachments\": {\n      \"type\": \"number\",\n      \"description\": \"The number of detach events for this period.\"\n    },\n    \"insertions\": {\n      \"type\": \"number\",\n      \"description\": \"The number of insertion events for this period.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-analytics-library-analytics-actions-by-component-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: LibraryAnalyticsActionsByComponent
---
