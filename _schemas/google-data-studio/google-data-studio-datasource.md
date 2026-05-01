---
description: Represents a Looker Studio data source, which connects to an external data provider and defines the schema of available fields. Data sources are a subtype of Asset with assetType DATA_SOURCE and can be configured through the Linking API or Community Connectors.
layout: schema
name: Looker Studio Data Source
properties_list:
- description: The asset type, always DATA_SOURCE for data source assets.
  name: assetType
  type: string
- description: The unique name (ID) of the data source.
  name: name
  type: string
- description: The display title of the data source.
  name: title
  type: string
- description: The email address of the data source owner.
  name: owner
  type: string
- description: The email address of the user who originally created the data source.
  name: creator
  type: string
- description: Timestamp when the data source was created, in RFC 3339 format.
  name: createTime
  type: string
- description: Timestamp when the data source was last modified, in RFC 3339 format.
  name: updateTime
  type: string
- description: Timestamp when the data source was last modified by the authenticated user, in RFC 3339 format.
  name: updateByMeTime
  type: string
- description: Timestamp when the data source was last viewed by the authenticated user, in RFC 3339 format.
  name: lastViewByMeTime
  type: string
- description: Indicates whether the data source is currently in the trash.
  name: trashed
  type: boolean
provider_name: Google Data Studio
provider_slug: google-data-studio
schema_file: json-schema/google-data-studio-datasource-schema.json
slug: google-data-studio-datasource
source_filename: google-data-studio-datasource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"google-data-studio-datasource-schema.json\",\n  \"title\": \"Looker Studio Data Source\",\n  \"description\": \"Represents a Looker Studio data source, which connects to an external data provider and defines the schema of available fields. Data sources are a subtype of Asset with assetType DATA_SOURCE and can be configured through the Linking API or Community Connectors.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"assetType\",\n    \"name\",\n    \"title\",\n    \"owner\",\n    \"creator\",\n    \"createTime\",\n    \"updateTime\"\n  ],\n  \"properties\": {\n    \"assetType\": {\n      \"type\": \"string\",\n      \"description\": \"The asset type, always DATA_SOURCE for data source assets.\",\n      \"const\": \"DATA_SOURCE\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name (ID) of the data source.\"\n    },\n    \"title\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The display title of the data source.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the data source owner.\",\n      \"format\": \"email\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user who originally created the data source.\",\n      \"format\": \"email\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the data source was created, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the data source was last modified, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"updateByMeTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the data source was last modified by the authenticated user, in RFC 3339 format.\",\n   \
  \   \"format\": \"date-time\"\n    },\n    \"lastViewByMeTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the data source was last viewed by the authenticated user, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"trashed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the data source is currently in the trash.\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/json-schema/google-data-studio-datasource-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data
- Reporting
- Visualization
title: Looker Studio Data Source
---
