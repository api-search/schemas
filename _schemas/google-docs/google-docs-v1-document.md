---
description: A Google Docs document. The Document resource represents the full content and metadata of a document.
layout: schema
name: Document
properties_list:
- description: Output only. The ID of the document.
  name: documentId
  type: string
- description: The title of the document.
  name: title
  type: string
- description: Tabs that are part of a document. Tabs can contain child tabs, creating a nested tab structure.
  name: tabs
  type: array
- description: Output only. The revision ID of the document. Can be used in update requests to specify which revision of a document to apply updates to, and how the request should behave if the document has been edi
  name: revisionId
  type: string
- description: Output only. The headers in the document, keyed by header ID.
  name: headers
  type: object
- description: Output only. The footers in the document, keyed by footer ID.
  name: footers
  type: object
- description: Output only. The footnotes in the document, keyed by footnote ID.
  name: footnotes
  type: object
- description: Output only. The suggested changes to the style of the document, keyed by suggestion ID.
  name: suggestedDocumentStyleChanges
  type: object
- description: Output only. The suggested changes to the named styles of the document, keyed by suggestion ID.
  name: suggestedNamedStylesChanges
  type: object
- description: Output only. The lists in the document, keyed by list ID.
  name: lists
  type: object
- description: Output only. The named ranges in the document, keyed by name.
  name: namedRanges
  type: object
- description: Output only. The inline objects in the document, keyed by object ID.
  name: inlineObjects
  type: object
- description: Output only. The positioned objects in the document, keyed by object ID.
  name: positionedObjects
  type: object
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-document-schema.json
slug: google-docs-v1-document
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Document\",\n  \"type\": \"object\",\n  \"description\": \"A Google Docs document. The Document resource represents the full content and metadata of a document.\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The ID of the document.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the document.\"\n    },\n    \"tabs\": {\n      \"type\": \"array\",\n      \"description\": \"Tabs that are part of a document. Tabs can contain child tabs, creating a nested tab structure.\"\n    },\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The revision ID of the document. Can be used in update requests to specify which revision of a document to apply updates to, and how the request should behave if the document has been edited since that revision.\"\n\
  \    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The headers in the document, keyed by header ID.\"\n    },\n    \"footers\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The footers in the document, keyed by footer ID.\"\n    },\n    \"footnotes\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The footnotes in the document, keyed by footnote ID.\"\n    },\n    \"suggestedDocumentStyleChanges\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The suggested changes to the style of the document, keyed by suggestion ID.\"\n    },\n    \"suggestedNamedStylesChanges\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The suggested changes to the named styles of the document, keyed by suggestion ID.\"\n    },\n    \"lists\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The lists in the document, keyed by list ID.\"\n    },\n    \"\
  namedRanges\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The named ranges in the document, keyed by name.\"\n    },\n    \"inlineObjects\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The inline objects in the document, keyed by object ID.\"\n    },\n    \"positionedObjects\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The positioned objects in the document, keyed by object ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-document-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: Document
---
