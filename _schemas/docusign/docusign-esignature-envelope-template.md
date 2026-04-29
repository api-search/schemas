---
description: A template that defines reusable documents, recipients, tabs, and routing for envelope workflows.
layout: schema
name: EnvelopeTemplate
properties_list:
- description: The unique identifier of the template.
  name: templateId
  type: string
- description: The URI for the template.
  name: uri
  type: string
- description: The name of the template.
  name: name
  type: string
- description: A description of the template.
  name: description
  type: string
- description: The date the template was created.
  name: created
  type: string
- description: The date the template was last modified.
  name: lastModified
  type: string
- description: The date the template was last used.
  name: lastUsed
  type: string
- description: Whether the template is shared.
  name: shared
  type: string
- description: The folder ID containing the template.
  name: folderId
  type: string
- description: The name of the folder containing the template.
  name: folderName
  type: string
- description: The default email subject for envelopes using this template.
  name: emailSubject
  type: string
- description: The default email body for envelopes using this template.
  name: emailBlurb
  type: string
- description: The signing location setting.
  name: signingLocation
  type: string
- description: The documents included in the template.
  name: documents
  type: array
- description: Template status.
  name: status
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-template-schema.json
slug: docusign-esignature-envelope-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopeTemplate\",\n  \"type\": \"object\",\n  \"description\": \"A template that defines reusable documents, recipients, tabs, and routing for envelope workflows.\",\n  \"properties\": {\n    \"templateId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the template.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI for the template.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the template.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the template.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"The date the template was created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"description\": \"The date the template was last modified.\"\n    },\n\
  \    \"lastUsed\": {\n      \"type\": \"string\",\n      \"description\": \"The date the template was last used.\"\n    },\n    \"shared\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the template is shared.\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"The folder ID containing the template.\"\n    },\n    \"folderName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the folder containing the template.\"\n    },\n    \"emailSubject\": {\n      \"type\": \"string\",\n      \"description\": \"The default email subject for envelopes using this template.\"\n    },\n    \"emailBlurb\": {\n      \"type\": \"string\",\n      \"description\": \"The default email body for envelopes using this template.\"\n    },\n    \"signingLocation\": {\n      \"type\": \"string\",\n      \"description\": \"The signing location setting.\"\n    },\n    \"documents\": {\n      \"type\": \"array\",\n      \"description\": \"The\
  \ documents included in the template.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Template status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-template-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopeTemplate
---
