---
description: ''
layout: schema
name: AssetDownloadResponse
properties_list:
- description: The unique identifier of the asset.
  name: assetID
  type: string
- description: The pre-signed URI to download the asset. Valid for a limited time.
  name: downloadUri
  type: string
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-asset-download-response-schema.json
slug: adobe-pdf-services-asset-download-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetDownloadResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the asset.\"\n    },\n    \"downloadUri\": {\n      \"type\": \"string\",\n      \"description\": \"The pre-signed URI to download the asset. Valid for a limited time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-asset-download-response-schema.json
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
title: AssetDownloadResponse
---
