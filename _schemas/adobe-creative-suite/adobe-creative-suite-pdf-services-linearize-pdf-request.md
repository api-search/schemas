---
description: Request body for linearizing a PDF for fast web view
layout: schema
name: LinearizePDFRequest
properties_list:
- description: Asset ID of the PDF to linearize
  name: assetID
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-linearize-pdf-request-schema.json
slug: adobe-creative-suite-pdf-services-linearize-pdf-request
source_filename: adobe-creative-suite-pdf-services-linearize-pdf-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-linearize-pdf-request-schema.json\",\n  \"title\": \"LinearizePDFRequest\",\n  \"description\": \"Request body for linearizing a PDF for fast web view\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"Asset ID of the PDF to linearize\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    }\n  },\n  \"required\": [\n    \"assetID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-linearize-pdf-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: LinearizePDFRequest
---
