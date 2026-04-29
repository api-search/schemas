---
description: Request message for BatchUpdatePresentation.
layout: schema
name: BatchUpdatePresentationRequest
properties_list:
- description: A list of updates to apply to the presentation.
  name: requests
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-batch-update-presentation-request-schema.json
slug: google-slides-batch-update-presentation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdatePresentationRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request message for BatchUpdatePresentation.\",\n  \"properties\": {\n    \"requests\": {\n      \"type\": \"array\",\n      \"description\": \"A list of updates to apply to the presentation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-batch-update-presentation-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: BatchUpdatePresentationRequest
---
