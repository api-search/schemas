---
description: The properties of a Page that are only relevant for pages with pageType NOTES.
layout: schema
name: NotesProperties
properties_list:
- description: The object ID of the shape on this notes page that contains the speaker notes for the corresponding slide.
  name: speakerNotesObjectId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-notes-properties-schema.json
slug: google-slides-notes-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotesProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of a Page that are only relevant for pages with pageType NOTES.\\n\",\n  \"properties\": {\n    \"speakerNotesObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the shape on this notes page that contains the speaker notes for the corresponding slide.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-notes-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: NotesProperties
---
