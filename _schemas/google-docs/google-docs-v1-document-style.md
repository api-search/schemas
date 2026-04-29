---
description: The style of the document, influencing the look of the document and any defaults for new content.
layout: schema
name: DocumentStyle
properties_list:
- description: The ID of the default header.
  name: defaultHeaderId
  type: string
- description: The ID of the default footer.
  name: defaultFooterId
  type: string
- description: The ID of the header used for even pages.
  name: evenPageHeaderId
  type: string
- description: The ID of the footer used for even pages.
  name: evenPageFooterId
  type: string
- description: The ID of the header used for the first page.
  name: firstPageHeaderId
  type: string
- description: The ID of the footer used for the first page.
  name: firstPageFooterId
  type: string
- description: Whether to use the first page header/footer IDs for the first page of the document.
  name: useFirstPageHeaderFooter
  type: boolean
- description: Whether to use the even page header/footer IDs for even pages.
  name: useEvenPageHeaderFooter
  type: boolean
- description: The page number from which to start counting the number of pages.
  name: pageNumberStart
  type: integer
- description: Whether to use custom header/footer margins.
  name: useCustomHeaderFooterMargins
  type: boolean
- description: Whether to flip the orientation of the page to landscape, which effectively swaps the width and height of the page size.
  name: flipPageOrientation
  type: boolean
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-document-style-schema.json
slug: google-docs-v1-document-style
source_filename: google-docs-v1-document-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DocumentStyle\",\n  \"type\": \"object\",\n  \"description\": \"The style of the document, influencing the look of the document and any defaults for new content.\",\n  \"properties\": {\n    \"defaultHeaderId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the default header.\"\n    },\n    \"defaultFooterId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the default footer.\"\n    },\n    \"evenPageHeaderId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the header used for even pages.\"\n    },\n    \"evenPageFooterId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the footer used for even pages.\"\n    },\n    \"firstPageHeaderId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the header used for the first page.\"\n    },\n    \"firstPageFooterId\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The ID of the footer used for the first page.\"\n    },\n    \"useFirstPageHeaderFooter\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use the first page header/footer IDs for the first page of the document.\"\n    },\n    \"useEvenPageHeaderFooter\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use the even page header/footer IDs for even pages.\"\n    },\n    \"pageNumberStart\": {\n      \"type\": \"integer\",\n      \"description\": \"The page number from which to start counting the number of pages.\"\n    },\n    \"useCustomHeaderFooterMargins\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use custom header/footer margins.\"\n    },\n    \"flipPageOrientation\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to flip the orientation of the page to landscape, which effectively swaps the width and height of the page size.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-document-style-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: DocumentStyle
---
