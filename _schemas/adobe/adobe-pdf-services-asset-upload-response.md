---
description: ''
layout: schema
name: AssetUploadResponse
properties_list:
- description: The unique identifier for the uploaded asset.
  name: assetID
  type: string
- description: The pre-signed URI to upload the file content via HTTP PUT. Valid for a limited time.
  name: uploadUri
  type: string
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-asset-upload-response-schema.json
slug: adobe-pdf-services-asset-upload-response
source_filename: adobe-pdf-services-asset-upload-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetUploadResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the uploaded asset.\"\n    },\n    \"uploadUri\": {\n      \"type\": \"string\",\n      \"description\": \"The pre-signed URI to upload the file content via HTTP PUT. Valid for a limited time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-asset-upload-response-schema.json
tags:
- Analytics
- Creative Cloud
- Digital Asset Management
- Document Services
- E-Commerce
- E-Signatures
- Experience Cloud
- Generative AI
- Marketing
- PDF
- Work Management
title: AssetUploadResponse
---
