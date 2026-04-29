---
description: Request body for generating a document from a template
layout: schema
name: DocumentGenerationRequest
properties_list:
- description: Asset ID of the Word document template
  name: assetID
  type: string
- description: Output format of the generated document
  name: outputFormat
  type: string
- description: JSON data object whose keys map to template tags in the document
  name: jsonDataForMerge
  type: object
- description: Whether to include non-tagged content as plain text additions
  name: notTaggedAdds
  type: boolean
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-document-generation-request-schema.json
slug: adobe-creative-suite-pdf-services-document-generation-request
source_filename: adobe-creative-suite-pdf-services-document-generation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-document-generation-request-schema.json\",\n  \"title\": \"DocumentGenerationRequest\",\n  \"description\": \"Request body for generating a document from a template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"Asset ID of the Word document template\",\n      \"example\": \"urn:aaid:AS:UE1:23c30ee0-2e4d-46d6-87f2-087832fca718\"\n    },\n    \"outputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Output format of the generated document\",\n      \"enum\": [\n        \"pdf\",\n        \"docx\"\n      ],\n      \"example\": \"pdf\"\n    },\n    \"jsonDataForMerge\": {\n      \"type\": \"object\",\n      \"description\": \"JSON data object whose keys map to template tags in\
  \ the document\",\n      \"additionalProperties\": true,\n      \"example\": {\n        \"customerName\": \"John Doe\",\n        \"invoiceDate\": \"2026-03-02\",\n        \"totalAmount\": 1500.0\n      }\n    },\n    \"notTaggedAdds\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include non-tagged content as plain text additions\",\n      \"default\": false,\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"assetID\",\n    \"outputFormat\",\n    \"jsonDataForMerge\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-document-generation-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: DocumentGenerationRequest
---
