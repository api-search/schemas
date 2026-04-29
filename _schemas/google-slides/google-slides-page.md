---
description: A page in a presentation.
layout: schema
name: Page
properties_list:
- description: The object ID for this page. Object IDs used by Page and PageElement share the same namespace.
  name: objectId
  type: string
- description: The type of the page.
  name: pageType
  type: string
- description: The page elements rendered on the page.
  name: pageElements
  type: array
- description: Output only. The revision ID of the presentation containing this page. Can be used in update requests to assert the presentation revision has not changed since the last read operation.
  name: revisionId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-page-schema.json
slug: google-slides-page
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Page\",\n  \"type\": \"object\",\n  \"description\": \"A page in a presentation.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID for this page. Object IDs used by Page and PageElement share the same namespace.\\n\"\n    },\n    \"pageType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the page.\"\n    },\n    \"pageElements\": {\n      \"type\": \"array\",\n      \"description\": \"The page elements rendered on the page.\"\n    },\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The revision ID of the presentation containing this page. Can be used in update requests to assert the presentation revision has not changed since the last read operation.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-page-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Page
---
