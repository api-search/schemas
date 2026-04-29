---
description: Position and size of a single element within a dashboard layout
layout: schema
name: DashboardLayoutComponent
properties_list:
- description: Unique identifier
  name: id
  type: string
- description: ID of the parent layout
  name: dashboard_layout_id
  type: string
- description: ID of the dashboard element this positions
  name: dashboard_element_id
  type: string
- description: Row position in the grid
  name: row
  type: integer
- description: Column position in the grid
  name: column
  type: integer
- description: Width in grid units
  name: width
  type: integer
- description: Height in grid units
  name: height
  type: integer
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-dashboard-layout-component-schema.json
slug: looker-dashboard-layout-component
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardLayoutComponent\",\n  \"type\": \"object\",\n  \"description\": \"Position and size of a single element within a dashboard layout\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier\"\n    },\n    \"dashboard_layout_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent layout\"\n    },\n    \"dashboard_element_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the dashboard element this positions\"\n    },\n    \"row\": {\n      \"type\": \"integer\",\n      \"description\": \"Row position in the grid\"\n    },\n    \"column\": {\n      \"type\": \"integer\",\n      \"description\": \"Column position in the grid\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width in grid units\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Height in grid units\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-dashboard-layout-component-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: DashboardLayoutComponent
---
