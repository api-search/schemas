---
description: A single tile on a dashboard. Each element can contain a query, a reference to a Look, a merge query, or text/markdown content.
layout: schema
name: DashboardElement
properties_list:
- description: Unique identifier for this element
  name: id
  type: string
- description: ID of the parent dashboard
  name: dashboard_id
  type: string
- description: ID of a Look to display in this tile
  name: look_id
  type: integer
- description: ID of a query to run in this tile
  name: query_id
  type: integer
- description: Element type
  name: type
  type: string
- description: Display title for this tile
  name: title
  type: string
- description: Whether the title is hidden
  name: title_hidden
  type: boolean
- description: Subtitle text displayed below the title
  name: subtitle_text
  type: string
- description: Body text for text-type elements
  name: body_text
  type: string
- description: Note text displayed on the tile
  name: note_text
  type: string
- description: How the note is displayed (above, below, hover)
  name: note_display
  type: string
- description: Note display state
  name: note_state
  type: string
- description: Result maker configuration for merged queries
  name: result_maker
  type: object
- description: Rich content JSON for advanced text elements
  name: rich_content_json
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-dashboard-element-schema.json
slug: looker-dashboard-element
source_filename: looker-dashboard-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardElement\",\n  \"type\": \"object\",\n  \"description\": \"A single tile on a dashboard. Each element can contain a query, a reference to a Look, a merge query, or text/markdown content.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this element\"\n    },\n    \"dashboard_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent dashboard\"\n    },\n    \"look_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of a Look to display in this tile\"\n    },\n    \"query_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of a query to run in this tile\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Element type\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title for this tile\"\n    },\n \
  \   \"title_hidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the title is hidden\"\n    },\n    \"subtitle_text\": {\n      \"type\": \"string\",\n      \"description\": \"Subtitle text displayed below the title\"\n    },\n    \"body_text\": {\n      \"type\": \"string\",\n      \"description\": \"Body text for text-type elements\"\n    },\n    \"note_text\": {\n      \"type\": \"string\",\n      \"description\": \"Note text displayed on the tile\"\n    },\n    \"note_display\": {\n      \"type\": \"string\",\n      \"description\": \"How the note is displayed (above, below, hover)\"\n    },\n    \"note_state\": {\n      \"type\": \"string\",\n      \"description\": \"Note display state\"\n    },\n    \"result_maker\": {\n      \"type\": \"object\",\n      \"description\": \"Result maker configuration for merged queries\"\n    },\n    \"rich_content_json\": {\n      \"type\": \"string\",\n      \"description\": \"Rich content JSON for advanced text elements\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-dashboard-element-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: DashboardElement
---
