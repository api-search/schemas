---
description: A single slide within an Apple Keynote presentation
layout: schema
name: Slide
properties_list:
- description: The 1-based position of the slide
  name: slideNumber
  type: integer
- description: The title displayed on the slide
  name: title
  type: string
- description: The slide layout name
  name: layout
  type: string
- description: Whether this slide is skipped during playback
  name: skipped
  type: boolean
- description: Presenter notes for the slide
  name: notes
  type: string
- description: Slide background color in hex
  name: backgroundColor
  type: string
provider_name: Apple Keynote
provider_slug: apple-keynote
schema_file: json-schema/apple-keynote-slide-schema.json
slug: apple-keynote-slide
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apple-keynote/refs/heads/main/json-schema/apple-keynote-slide-schema.json\",\n  \"title\": \"Slide\",\n  \"description\": \"A single slide within an Apple Keynote presentation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"slideNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"The 1-based position of the slide\",\n      \"example\": 1\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title displayed on the slide\",\n      \"example\": \"Q4 Business Review\"\n    },\n    \"layout\": {\n      \"type\": \"string\",\n      \"description\": \"The slide layout name\",\n      \"example\": \"Title - Center\"\n    },\n    \"skipped\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this slide is skipped during playback\",\n      \"example\": false\n    },\n    \"notes\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Presenter notes for the slide\",\n      \"example\": \"Welcome to the review.\"\n    },\n    \"backgroundColor\": {\n      \"type\": \"string\",\n      \"description\": \"Slide background color in hex\",\n      \"example\": \"#FFFFFF\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple-keynote/refs/heads/main/json-schema/apple-keynote-slide-schema.json
tags:
- Apple
- Design
- iWork
- Presentations
- Productivity
- Slides
title: Slide
---
