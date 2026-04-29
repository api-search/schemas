---
description: Reference to an input image for generative operations
layout: schema
name: InputImageReference
properties_list:
- description: Source of the input image
  name: source
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-input-image-reference-schema.json
slug: adobe-creative-suite-firefly-input-image-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-input-image-reference-schema.json\",\n  \"title\": \"InputImageReference\",\n  \"description\": \"Reference to an input image for generative operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"Source of the input image\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"Publicly accessible URL of the input image\",\n          \"example\": \"https://my-bucket.s3.amazonaws.com/source-image.jpg\"\n        },\n        \"uploadId\": {\n          \"type\": \"string\",\n          \"description\": \"Upload ID for a previously uploaded image via the Firefly upload API\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"source\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-input-image-reference-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: InputImageReference
---
