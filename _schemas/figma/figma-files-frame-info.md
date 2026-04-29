---
description: Information about the containing frame.
layout: schema
name: FrameInfo
properties_list:
- description: The ID of the containing frame.
  name: nodeId
  type: string
- description: The name of the containing frame.
  name: name
  type: string
- description: The background color of the containing frame.
  name: backgroundColor
  type: string
- description: The ID of the page containing the frame.
  name: pageId
  type: string
- description: The name of the page containing the frame.
  name: pageName
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-files-frame-info-schema.json
slug: figma-files-frame-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FrameInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information about the containing frame.\",\n  \"properties\": {\n    \"nodeId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the containing frame.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the containing frame.\"\n    },\n    \"backgroundColor\": {\n      \"type\": \"string\",\n      \"description\": \"The background color of the containing frame.\"\n    },\n    \"pageId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the page containing the frame.\"\n    },\n    \"pageName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the page containing the frame.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-files-frame-info-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: FrameInfo
---
