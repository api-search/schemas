---
description: Summary information about a template operation.
layout: schema
name: TemplateSummary
properties_list:
- description: The unique identifier of the template.
  name: templateId
  type: string
- description: The name of the template.
  name: name
  type: string
- description: The URI for the template.
  name: uri
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-template-summary-schema.json
slug: docusign-esignature-template-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TemplateSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary information about a template operation.\",\n  \"properties\": {\n    \"templateId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the template.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the template.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI for the template.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-template-summary-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: TemplateSummary
---
