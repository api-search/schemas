---
description: The crop properties of an object enclosed in a container.
layout: schema
name: CropProperties
properties_list:
- description: The offset specifies the left edge of the crop rectangle that is located to the right of the original bounding rectangle left edge, relative to the object's original width.
  name: leftOffset
  type: number
- description: The offset specifies how far inward the right edge of the crop rectangle is from the right edge of the original bounding rectangle.
  name: rightOffset
  type: number
- description: The offset specifies how far inward the top edge of the crop rectangle is from the top edge of the original bounding rectangle.
  name: topOffset
  type: number
- description: The offset specifies how far inward the bottom edge of the crop rectangle is from the bottom edge of the original bounding rectangle.
  name: bottomOffset
  type: number
- description: The rotation angle of the crop window around its center, in radians.
  name: angle
  type: number
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-crop-properties-schema.json
slug: google-slides-crop-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CropProperties\",\n  \"type\": \"object\",\n  \"description\": \"The crop properties of an object enclosed in a container.\\n\",\n  \"properties\": {\n    \"leftOffset\": {\n      \"type\": \"number\",\n      \"description\": \"The offset specifies the left edge of the crop rectangle that is located to the right of the original bounding rectangle left edge, relative to the object's original width.\\n\"\n    },\n    \"rightOffset\": {\n      \"type\": \"number\",\n      \"description\": \"The offset specifies how far inward the right edge of the crop rectangle is from the right edge of the original bounding rectangle.\\n\"\n    },\n    \"topOffset\": {\n      \"type\": \"number\",\n      \"description\": \"The offset specifies how far inward the top edge of the crop rectangle is from the top edge of the original bounding rectangle.\\n\"\n    },\n    \"bottomOffset\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"The offset specifies how far inward the bottom edge of the crop rectangle is from the bottom edge of the original bounding rectangle.\\n\"\n    },\n    \"angle\": {\n      \"type\": \"number\",\n      \"description\": \"The rotation angle of the crop window around its center, in radians.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-crop-properties-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: CropProperties
---
