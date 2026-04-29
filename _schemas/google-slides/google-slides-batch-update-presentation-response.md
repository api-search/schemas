---
description: Response message from a BatchUpdatePresentation request.
layout: schema
name: BatchUpdatePresentationResponse
properties_list:
- description: The presentation the updates were applied to.
  name: presentationId
  type: string
- description: The reply of the updates. This maps 1:1 with the updates, although replies to some requests may be empty.
  name: replies
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-batch-update-presentation-response-schema.json
slug: google-slides-batch-update-presentation-response
source_filename: google-slides-batch-update-presentation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdatePresentationResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response message from a BatchUpdatePresentation request.\",\n  \"properties\": {\n    \"presentationId\": {\n      \"type\": \"string\",\n      \"description\": \"The presentation the updates were applied to.\"\n    },\n    \"replies\": {\n      \"type\": \"array\",\n      \"description\": \"The reply of the updates. This maps 1:1 with the updates, although replies to some requests may be empty.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-batch-update-presentation-response-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: BatchUpdatePresentationResponse
---
