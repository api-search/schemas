---
description: ''
layout: schema
name: AvailableContentStates
properties_list:
- description: Space suggested content states that can be used in the space. This can be null if space content states are disabled in the space. This list can be empty if there are no space content states defined in
  name: spaceContentStates
  type: array
- description: 'Custom content states that can be used by the user on the content of this call. This can be null if custom content states are disabled in the space of the content. This list can be empty if there are '
  name: customContentStates
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-available-content-states-schema.json
slug: atlassian-confluence-content-available-content-states
source_filename: atlassian-confluence-content-available-content-states-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AvailableContentStates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceContentStates\": {\n      \"type\": \"array\",\n      \"description\": \"Space suggested content states that can be used in the space. This can be null if space content states are disabled in the space.\\nThis list can be empty if there are no space content states defined in the space.\\nAll spaces start with 3 default space content states, and this can be modified in the UI under space settings.\"\n    },\n    \"customContentStates\": {\n      \"type\": \"array\",\n      \"description\": \"Custom content states that can be used by the user on the content of this call.\\nThis can be null if custom content states are disabled in the space of the content.\\nThis list can be empty if there are no custom content states defined by the user.\\nThis will at most have 3 of the most recently published content states.\
  \ \\nOnly the calling user has access to place these states on content, but all users can see these states once they are placed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-available-content-states-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: AvailableContentStates
---
