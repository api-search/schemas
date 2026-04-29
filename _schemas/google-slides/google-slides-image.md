---
description: A PageElement kind representing an image.
layout: schema
name: Image
properties_list:
- description: An URL to an image with a default lifetime of 30 minutes. This URL is tagged with the account of the requester.
  name: contentUrl
  type: string
- description: The source URL is the URL used to insert the image. The source URL can be empty.
  name: sourceUrl
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-image-schema.json
slug: google-slides-image
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Image\",\n  \"type\": \"object\",\n  \"description\": \"A PageElement kind representing an image.\\n\",\n  \"properties\": {\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"An URL to an image with a default lifetime of 30 minutes. This URL is tagged with the account of the requester.\\n\"\n    },\n    \"sourceUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The source URL is the URL used to insert the image. The source URL can be empty.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-image-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Image
---
