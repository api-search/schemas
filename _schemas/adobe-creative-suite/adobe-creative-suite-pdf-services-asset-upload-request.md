---
description: Request to initiate an asset upload
layout: schema
name: AssetUploadRequest
properties_list:
- description: MIME type of the file to be uploaded
  name: mediaType
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-asset-upload-request-schema.json
slug: adobe-creative-suite-pdf-services-asset-upload-request
source_filename: adobe-creative-suite-pdf-services-asset-upload-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-asset-upload-request-schema.json\",\n  \"title\": \"AssetUploadRequest\",\n  \"description\": \"Request to initiate an asset upload\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the file to be uploaded\",\n      \"example\": \"application/vnd.openxmlformats-officedocument.wordprocessingml.document\"\n    }\n  },\n  \"required\": [\n    \"mediaType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-asset-upload-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: AssetUploadRequest
---
