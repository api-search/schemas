---
description: A Google Slides presentation.
layout: schema
name: Presentation
properties_list:
- description: The ID of the presentation.
  name: presentationId
  type: string
- description: The title of the presentation.
  name: title
  type: string
- description: The slides in the presentation. A slide inherits properties from a slide layout.
  name: slides
  type: array
- description: The slide masters in the presentation. A slide master contains all common page elements and the common properties for a set of layouts.
  name: masters
  type: array
- description: The layouts in the presentation. A layout is a template that determines how content is arranged and styled on the slides that inherit from that layout.
  name: layouts
  type: array
- description: The locale of the presentation as an IETF BCP 47 language tag.
  name: locale
  type: string
- description: 'Output only. The revision ID of the presentation. Can be used in update requests to assert that the presentation revision has not changed since the last read operation. Only populated if the user has '
  name: revisionId
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-presentation-schema.json
slug: google-slides-presentation
source_filename: google-slides-presentation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Presentation\",\n  \"type\": \"object\",\n  \"description\": \"A Google Slides presentation.\",\n  \"properties\": {\n    \"presentationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the presentation.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the presentation.\"\n    },\n    \"slides\": {\n      \"type\": \"array\",\n      \"description\": \"The slides in the presentation. A slide inherits properties from a slide layout.\\n\"\n    },\n    \"masters\": {\n      \"type\": \"array\",\n      \"description\": \"The slide masters in the presentation. A slide master contains all common page elements and the common properties for a set of layouts.\\n\"\n    },\n    \"layouts\": {\n      \"type\": \"array\",\n      \"description\": \"The layouts in the presentation. A layout is a template that determines how content is arranged\
  \ and styled on the slides that inherit from that layout.\\n\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"The locale of the presentation as an IETF BCP 47 language tag.\\n\"\n    },\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The revision ID of the presentation. Can be used in update requests to assert that the presentation revision has not changed since the last read operation. Only populated if the user has edit access to the presentation. The revision ID is not a sequential number but an opaque string. The format may change over time. A returned revision ID is only guaranteed to be valid for 24 hours after it has been returned and cannot be shared across users.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-presentation-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Presentation
---
