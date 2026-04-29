---
description: Replaces an existing image with a new image. Replacing an image removes some image effects from the existing image in order to mirror the behavior of the Docs editor.
layout: schema
name: ReplaceImageRequest
properties_list:
- description: The ID of the existing image that will be replaced.
  name: imageObjectId
  type: string
- description: The URI of the new image. The image is fetched once at insertion time and a copy is stored for display inside the document.
  name: uri
  type: string
- description: The replacement method.
  name: imageReplaceMethod
  type: string
- description: The tab that the image to be replaced is in.
  name: tabId
  type: string
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-replace-image-request-schema.json
slug: google-docs-v1-replace-image-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplaceImageRequest\",\n  \"type\": \"object\",\n  \"description\": \"Replaces an existing image with a new image. Replacing an image removes some image effects from the existing image in order to mirror the behavior of the Docs editor.\",\n  \"properties\": {\n    \"imageObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the existing image that will be replaced.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI of the new image. The image is fetched once at insertion time and a copy is stored for display inside the document.\"\n    },\n    \"imageReplaceMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The replacement method.\"\n    },\n    \"tabId\": {\n      \"type\": \"string\",\n      \"description\": \"The tab that the image to be replaced is in.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-replace-image-request-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: ReplaceImageRequest
---
