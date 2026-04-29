---
description: The properties for one end of a Line connection.
layout: schema
name: LineConnection
properties_list:
- description: The object ID of the connected page element.
  name: connectedObjectId
  type: string
- description: The index of the connection site on the connected page element.
  name: connectionSiteIndex
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-line-connection-schema.json
slug: google-slides-line-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LineConnection\",\n  \"type\": \"object\",\n  \"description\": \"The properties for one end of a Line connection.\",\n  \"properties\": {\n    \"connectedObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the connected page element.\"\n    },\n    \"connectionSiteIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the connection site on the connected page element.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-line-connection-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: LineConnection
---
