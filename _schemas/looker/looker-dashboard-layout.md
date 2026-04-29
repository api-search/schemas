---
description: Layout configuration for a dashboard defining tile positions
layout: schema
name: DashboardLayout
properties_list:
- description: Unique identifier for this layout
  name: id
  type: string
- description: ID of the parent dashboard
  name: dashboard_id
  type: string
- description: Layout type
  name: type
  type: string
- description: Whether this is the active layout
  name: active
  type: boolean
- description: Width of each column in the grid
  name: column_width
  type: integer
- description: Total width of the layout
  name: width
  type: integer
- description: Positioning of elements within this layout
  name: dashboard_layout_components
  type: array
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-dashboard-layout-schema.json
slug: looker-dashboard-layout
source_filename: looker-dashboard-layout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardLayout\",\n  \"type\": \"object\",\n  \"description\": \"Layout configuration for a dashboard defining tile positions\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this layout\"\n    },\n    \"dashboard_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent dashboard\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Layout type\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the active layout\"\n    },\n    \"column_width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width of each column in the grid\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Total width of the layout\"\n    },\n    \"dashboard_layout_components\": {\n      \"type\": \"array\",\n     \
  \ \"description\": \"Positioning of elements within this layout\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-dashboard-layout-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: DashboardLayout
---
