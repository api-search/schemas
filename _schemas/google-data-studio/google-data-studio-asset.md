---
description: Represents a Looker Studio asset such as a report or data source. Assets are the primary resources managed through the Looker Studio API and can be searched, shared, and have their permissions managed programmatically.
layout: schema
name: Looker Studio Asset
properties_list:
- description: The type of the Looker Studio asset.
  name: assetType
  type: string
- description: The unique name (ID) of the asset. This serves as the primary identifier when referencing the asset in API calls.
  name: name
  type: string
- description: The display title of the asset as shown in the Looker Studio interface.
  name: title
  type: string
- description: Description of the asset. Only supported for REPORT asset type.
  name: description
  type: string
- description: The email address of the asset owner.
  name: owner
  type: string
- description: The email address of the user who originally created the asset.
  name: creator
  type: string
- description: Timestamp when the asset was created, in RFC 3339 format.
  name: createTime
  type: string
- description: Timestamp when the asset was last modified by any user, in RFC 3339 format.
  name: updateTime
  type: string
- description: Timestamp when the asset was last modified by the user making the API call, in RFC 3339 format.
  name: updateByMeTime
  type: string
- description: Timestamp when the asset was last viewed by the user making the API call, in RFC 3339 format.
  name: lastViewByMeTime
  type: string
- description: Indicates whether the asset is currently in the trash.
  name: trashed
  type: boolean
provider_name: Google Data Studio
provider_slug: google-data-studio
schema_file: json-schema/google-data-studio-asset-schema.json
slug: google-data-studio-asset
source_filename: google-data-studio-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"google-data-studio-asset-schema.json\",\n  \"title\": \"Looker Studio Asset\",\n  \"description\": \"Represents a Looker Studio asset such as a report or data source. Assets are the primary resources managed through the Looker Studio API and can be searched, shared, and have their permissions managed programmatically.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"assetType\",\n    \"name\",\n    \"title\",\n    \"owner\",\n    \"creator\",\n    \"createTime\",\n    \"updateTime\"\n  ],\n  \"properties\": {\n    \"assetType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the Looker Studio asset.\",\n      \"enum\": [\n        \"REPORT\",\n        \"DATA_SOURCE\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name (ID) of the asset. This serves as the primary identifier when referencing the asset in API calls.\"\
  \n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the asset as shown in the Looker Studio interface.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the asset. Only supported for REPORT asset type.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the asset owner.\",\n      \"format\": \"email\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user who originally created the asset.\",\n      \"format\": \"email\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the asset was created, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the asset was last modified by any user, in RFC 3339 format.\",\n      \"format\"\
  : \"date-time\"\n    },\n    \"updateByMeTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the asset was last modified by the user making the API call, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"lastViewByMeTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the asset was last viewed by the user making the API call, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"trashed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the asset is currently in the trash.\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/json-schema/google-data-studio-asset-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data
- Reporting
- Visualization
title: Looker Studio Asset
---
