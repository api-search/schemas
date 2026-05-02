---
description: Represents a Looker Studio asset such as a report or data source. Assets are the primary objects managed through the Looker Studio API.
layout: schema
name: Looker Studio Asset
properties_list:
- description: The resource name of the asset, serving as its unique identifier.
  name: name
  type: string
- description: The type of Looker Studio asset.
  name: assetType
  type: string
- description: The display title of the asset as shown in the Looker Studio interface.
  name: title
  type: string
- description: A text description of the asset. Available for reports only.
  name: description
  type: string
- description: The email address of the asset owner who has full control over the asset.
  name: owner
  type: string
- description: The email address of the user who originally created the asset.
  name: creator
  type: string
- description: The timestamp when the asset was created, in RFC 3339 format.
  name: createTime
  type: string
- description: The timestamp when the asset was last modified by any user, in RFC 3339 format.
  name: updateTime
  type: string
- description: The timestamp when the authenticated user last modified the asset.
  name: updateByMeTime
  type: string
- description: The timestamp when the authenticated user last viewed the asset.
  name: lastViewByMeTime
  type: string
- description: Whether the asset has been moved to the trash.
  name: trashed
  type: boolean
provider_name: Looker Studio
provider_slug: looker-studio
schema_file: json-schema/looker-studio-asset-schema.json
slug: looker-studio-asset
source_filename: looker-studio-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/looker-studio/json-schema/looker-studio-asset-schema.json\",\n  \"title\": \"Looker Studio Asset\",\n  \"description\": \"Represents a Looker Studio asset such as a report or data source. Assets are the primary objects managed through the Looker Studio API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the asset, serving as its unique identifier.\"\n    },\n    \"assetType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of Looker Studio asset.\",\n      \"enum\": [\n        \"REPORT\",\n        \"DATA_SOURCE\"\n      ]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the asset as shown in the Looker Studio interface.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"A text description of the asset. Available for reports only.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the asset owner who has full control over the asset.\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user who originally created the asset.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the asset was created, in RFC 3339 format.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the asset was last modified by any user, in RFC 3339 format.\"\n    },\n    \"updateByMeTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the authenticated user last modified the\
  \ asset.\"\n    },\n    \"lastViewByMeTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the authenticated user last viewed the asset.\"\n    },\n    \"trashed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the asset has been moved to the trash.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"assetType\",\n    \"title\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/json-schema/looker-studio-asset-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
title: Looker Studio Asset
---
