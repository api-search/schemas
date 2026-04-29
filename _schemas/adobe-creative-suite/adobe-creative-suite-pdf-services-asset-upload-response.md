---
description: Response containing the upload URI and asset ID
layout: schema
name: AssetUploadResponse
properties_list:
- description: Asset ID to reference in subsequent operations
  name: assetID
  type: string
- description: Pre-signed URI to PUT the file content to
  name: uploadUri
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-asset-upload-response-schema.json
slug: adobe-creative-suite-pdf-services-asset-upload-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-asset-upload-response-schema.json\",\n  \"title\": \"AssetUploadResponse\",\n  \"description\": \"Response containing the upload URI and asset ID\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"Asset ID to reference in subsequent operations\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    },\n    \"uploadUri\": {\n      \"type\": \"string\",\n      \"description\": \"Pre-signed URI to PUT the file content to\",\n      \"example\": \"https://dcplatformstorageservice-us-east-1.s3-accelerate.amazonaws.com/...\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-asset-upload-response-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: AssetUploadResponse
---
