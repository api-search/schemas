---
description: ''
layout: schema
name: SpaceSettings
properties_list:
- description: Defines whether an override for the space home should be used. This is used in conjunction with a space theme provided by an app. For example, if this property is set to true, a theme can display a pa
  name: routeOverrideEnabled
  type: boolean
- description: ''
  name: editor
  type: object
- description: ''
  name: spaceKey
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-space-settings-schema.json
slug: atlassian-confluence-content-space-settings
source_filename: atlassian-confluence-content-space-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpaceSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"routeOverrideEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Defines whether an override for the space home should be used. This is\\nused in conjunction with a space theme provided by an app. For\\nexample, if this property is set to true, a theme can display a page\\nother than the space homepage when users visit the root URL for a\\nspace. This property allows apps to provide content-only theming\\nwithout overriding the space home.\"\n    },\n    \"editor\": {\n      \"type\": \"object\"\n    },\n    \"spaceKey\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-space-settings-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: SpaceSettings
---
