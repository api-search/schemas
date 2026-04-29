---
description: Metadata and download reference for an uploaded asset
layout: schema
name: Asset
properties_list:
- description: Unique identifier for the asset
  name: assetID
  type: string
- description: MIME type of the asset
  name: mediaType
  type: string
- description: Temporary signed URL to download the asset
  name: downloadUri
  type: string
- description: File size in bytes
  name: size
  type: integer
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-asset-schema.json
slug: adobe-creative-suite-pdf-services-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-asset-schema.json\",\n  \"title\": \"Asset\",\n  \"description\": \"Metadata and download reference for an uploaded asset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the asset\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    },\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the asset\",\n      \"example\": \"application/pdf\"\n    },\n    \"downloadUri\": {\n      \"type\": \"string\",\n      \"description\": \"Temporary signed URL to download the asset\",\n      \"example\": \"https://dcplatformstorageservice-us-east-1.s3-accelerate.amazonaws.com/...\"\n    },\n    \"size\": {\n      \"\
  type\": \"integer\",\n      \"description\": \"File size in bytes\",\n      \"example\": 204800\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-asset-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: Asset
---
