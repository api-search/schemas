---
description: A composite template that combines server templates and inline templates for complex envelope workflows.
layout: schema
name: CompositeTemplate
properties_list:
- description: Unique identifier for the composite template.
  name: compositeTemplateId
  type: string
- description: ''
  name: serverTemplates
  type: array
- description: ''
  name: inlineTemplates
  type: array
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-composite-template-schema.json
slug: docusign-esignature-composite-template
source_filename: docusign-esignature-composite-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompositeTemplate\",\n  \"type\": \"object\",\n  \"description\": \"A composite template that combines server templates and inline templates for complex envelope workflows.\",\n  \"properties\": {\n    \"compositeTemplateId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the composite template.\"\n    },\n    \"serverTemplates\": {\n      \"type\": \"array\"\n    },\n    \"inlineTemplates\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-composite-template-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: CompositeTemplate
---
