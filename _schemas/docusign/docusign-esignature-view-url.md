---
description: Contains a URL for an embedded view.
layout: schema
name: ViewUrl
properties_list:
- description: The URL for the embedded view. This URL is time-limited and should be used immediately.
  name: url
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-view-url-schema.json
slug: docusign-esignature-view-url
source_filename: docusign-esignature-view-url-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ViewUrl\",\n  \"type\": \"object\",\n  \"description\": \"Contains a URL for an embedded view.\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL for the embedded view. This URL is time-limited and should be used immediately.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-view-url-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: ViewUrl
---
