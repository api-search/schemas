---
description: Request body for auto-tagging a PDF for accessibility
layout: schema
name: AutoTagRequest
properties_list:
- description: Asset ID of the PDF to auto-tag
  name: assetID
  type: string
- description: Whether to generate an accessibility report alongside the tagged PDF
  name: generateReport
  type: boolean
- description: Whether to shift heading levels in the output for better document structure
  name: shiftHeadings
  type: boolean
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-auto-tag-request-schema.json
slug: adobe-creative-suite-pdf-services-auto-tag-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-auto-tag-request-schema.json\",\n  \"title\": \"AutoTagRequest\",\n  \"description\": \"Request body for auto-tagging a PDF for accessibility\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"Asset ID of the PDF to auto-tag\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    },\n    \"generateReport\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to generate an accessibility report alongside the tagged PDF\",\n      \"default\": false,\n      \"example\": true\n    },\n    \"shiftHeadings\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to shift heading levels in the output for better document structure\",\n      \"default\"\
  : false,\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"assetID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-auto-tag-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: AutoTagRequest
---
