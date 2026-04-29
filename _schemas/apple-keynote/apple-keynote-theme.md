---
description: An Apple Keynote theme defining the visual style of a presentation
layout: schema
name: Theme
properties_list:
- description: Display name of the theme
  name: name
  type: string
- description: Unique theme identifier
  name: identifier
  type: string
- description: Theme category (Basic, Bold, etc.)
  name: category
  type: string
- description: Primary colors used in theme
  name: colorScheme
  type: array
- description: Default font family for the theme
  name: fontFamily
  type: string
provider_name: Apple Keynote
provider_slug: apple-keynote
schema_file: json-schema/apple-keynote-theme-schema.json
slug: apple-keynote-theme
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apple-keynote/refs/heads/main/json-schema/apple-keynote-theme-schema.json\",\n  \"title\": \"Theme\",\n  \"description\": \"An Apple Keynote theme defining the visual style of a presentation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the theme\",\n      \"example\": \"White\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique theme identifier\",\n      \"example\": \"com.apple.themes.white\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Theme category (Basic, Bold, etc.)\",\n      \"example\": \"Basic\"\n    },\n    \"colorScheme\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Primary colors used in theme\"\
  \n    },\n    \"fontFamily\": {\n      \"type\": \"string\",\n      \"description\": \"Default font family for the theme\",\n      \"example\": \"San Francisco\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple-keynote/refs/heads/main/json-schema/apple-keynote-theme-schema.json
tags:
- Apple
- Design
- iWork
- Presentations
- Productivity
- Slides
title: Theme
---
