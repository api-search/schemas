---
description: ''
layout: schema
name: ContentStateSettings
properties_list:
- description: Whether users can place any content states on content
  name: contentStatesAllowed
  type: boolean
- description: Whether users can place their custom states on content
  name: customContentStatesAllowed
  type: boolean
- description: Whether users can place space suggested states on content
  name: spaceContentStatesAllowed
  type: boolean
- description: space suggested content states that users can choose from
  name: spaceContentStates
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-space-content-state-settings-schema.json
slug: atlassian-confluence-space-content-state-settings
source_filename: atlassian-confluence-space-content-state-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentStateSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contentStatesAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether users can place any content states on content\"\n    },\n    \"customContentStatesAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether users can place their custom states on content\"\n    },\n    \"spaceContentStatesAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether users can place space suggested states on content\"\n    },\n    \"spaceContentStates\": {\n      \"type\": \"array\",\n      \"description\": \"space suggested content states that users can choose from\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-space-content-state-settings-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentStateSettings
---
