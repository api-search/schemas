---
description: A visual element rendered on a page.
layout: schema
name: PageElement
properties_list:
- description: The object ID for this page element.
  name: objectId
  type: string
- description: The title of the page element for accessibility.
  name: title
  type: string
- description: The description of the page element for accessibility.
  name: description
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-page-element-schema.json
slug: google-slides-page-element
source_filename: google-slides-page-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageElement\",\n  \"type\": \"object\",\n  \"description\": \"A visual element rendered on a page.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID for this page element.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the page element for accessibility.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the page element for accessibility.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-page-element-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: PageElement
---
