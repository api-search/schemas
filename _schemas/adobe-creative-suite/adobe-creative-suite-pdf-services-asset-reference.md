---
description: Reference to an existing uploaded asset
layout: schema
name: AssetReference
properties_list:
- description: ID of the asset returned by the upload endpoint
  name: assetID
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-asset-reference-schema.json
slug: adobe-creative-suite-pdf-services-asset-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-asset-reference-schema.json\",\n  \"title\": \"AssetReference\",\n  \"description\": \"Reference to an existing uploaded asset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the asset returned by the upload endpoint\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    }\n  },\n  \"required\": [\n    \"assetID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-asset-reference-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: AssetReference
---
