---
description: Writable fields for creating or updating a dashboard
layout: schema
name: WriteDashboard
properties_list:
- description: Display title
  name: title
  type: string
- description: Description of the dashboard
  name: description
  type: string
- description: Space (folder) ID
  name: space_id
  type: string
- description: Folder ID
  name: folder_id
  type: string
- description: Timezone for queries
  name: query_timezone
  type: string
- description: CSS background color
  name: background_color
  type: string
- description: Default text color for text tiles
  name: text_tile_text_color
  type: string
- description: Default background color for tiles
  name: tile_background_color
  type: string
- description: Default text color for tiles
  name: tile_text_color
  type: string
- description: Whether the dashboard is hidden
  name: hidden
  type: boolean
- description: Auto-refresh interval
  name: refresh_interval
  type: string
- description: Tile load configuration
  name: load_configuration
  type: string
- description: Preferred viewer type
  name: preferred_viewer
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-write-dashboard-schema.json
slug: looker-write-dashboard
source_filename: looker-write-dashboard-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WriteDashboard\",\n  \"type\": \"object\",\n  \"description\": \"Writable fields for creating or updating a dashboard\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the dashboard\"\n    },\n    \"space_id\": {\n      \"type\": \"string\",\n      \"description\": \"Space (folder) ID\"\n    },\n    \"folder_id\": {\n      \"type\": \"string\",\n      \"description\": \"Folder ID\"\n    },\n    \"query_timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for queries\"\n    },\n    \"background_color\": {\n      \"type\": \"string\",\n      \"description\": \"CSS background color\"\n    },\n    \"text_tile_text_color\": {\n      \"type\": \"string\",\n      \"description\": \"Default text color for text tiles\"\
  \n    },\n    \"tile_background_color\": {\n      \"type\": \"string\",\n      \"description\": \"Default background color for tiles\"\n    },\n    \"tile_text_color\": {\n      \"type\": \"string\",\n      \"description\": \"Default text color for tiles\"\n    },\n    \"hidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dashboard is hidden\"\n    },\n    \"refresh_interval\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-refresh interval\"\n    },\n    \"load_configuration\": {\n      \"type\": \"string\",\n      \"description\": \"Tile load configuration\"\n    },\n    \"preferred_viewer\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred viewer type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-write-dashboard-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: WriteDashboard
---
