---
description: ''
layout: schema
name: ContentBlueprintDraft
properties_list:
- description: The version for the new content.
  name: version
  type: object
- description: The title of the content. If you don't want to change the title, set this to the current title of the draft.
  name: title
  type: string
- description: The type of content. Set this to `page`.
  name: type
  type: string
- description: The status of the content. Set this to `current` or omit it altogether.
  name: status
  type: string
- description: The space for the content.
  name: space
  type: object
- description: The new ancestor (i.e. parent page) for the content. If you have specified an ancestor, you must also specify a `space` property in the request body for the space that the ancestor is in. Note, if you
  name: ancestors
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-blueprint-draft-schema.json
slug: atlassian-confluence-content-content-blueprint-draft
source_filename: atlassian-confluence-content-content-blueprint-draft-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentBlueprintDraft\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"object\",\n      \"description\": \"The version for the new content.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the content. If you don't want to change the title,\\nset this to the current title of the draft.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of content. Set this to `page`.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the content. Set this to `current` or omit it altogether.\"\n    },\n    \"space\": {\n      \"type\": \"object\",\n      \"description\": \"The space for the content.\"\n    },\n    \"ancestors\": {\n      \"type\": \"array\",\n      \"description\": \"The new ancestor (i.e. parent page) for the content. If\
  \ you have\\nspecified an ancestor, you must also specify a `space` property\\nin the request body for the space that the ancestor is in.\\n\\nNote, if you specify more than one ancestor, the last ID in the array\\nwill be selected as the parent page for the content.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-blueprint-draft-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentBlueprintDraft
---
