---
description: Updates the position of slides in the presentation.
layout: schema
name: UpdateSlidesPositionRequest
properties_list:
- description: The IDs of the slides in the presentation that should be moved.
  name: slideObjectIds
  type: array
- description: The index where the slides should be inserted, based on the slide arrangement before the move takes place.
  name: insertionIndex
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-slides-position-request-schema.json
slug: google-slides-update-slides-position-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateSlidesPositionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the position of slides in the presentation.\",\n  \"properties\": {\n    \"slideObjectIds\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of the slides in the presentation that should be moved.\"\n    },\n    \"insertionIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The index where the slides should be inserted, based on the slide arrangement before the move takes place.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-slides-position-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdateSlidesPositionRequest
---
