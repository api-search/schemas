---
description: The envelope definition object that contains all the properties needed to create and send an envelope.
layout: schema
name: EnvelopeDefinition
properties_list:
- description: The subject line of the email sent to recipients.
  name: emailSubject
  type: string
- description: The body text of the email sent to recipients.
  name: emailBlurb
  type: string
- description: The envelope status. Set to "sent" to send the envelope immediately, or "created" to save as a draft.
  name: status
  type: string
- description: The ID of a template to use as the basis for the envelope. When specified, the template's documents, recipients, and tabs are merged with any specified in the request.
  name: templateId
  type: string
- description: Template role assignments that map recipients to template roles when using a templateId.
  name: templateRoles
  type: array
- description: The documents to include in the envelope.
  name: documents
  type: array
- description: An array of composite template objects that combine server templates and inline templates for complex workflows.
  name: compositeTemplates
  type: array
- description: The ID of the brand to apply to the envelope.
  name: brandId
  type: string
- description: When true, the envelope ID is stamped in the document margins.
  name: envelopeIdStamping
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-definition-schema.json
slug: docusign-esignature-envelope-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopeDefinition\",\n  \"type\": \"object\",\n  \"description\": \"The envelope definition object that contains all the properties needed to create and send an envelope.\",\n  \"properties\": {\n    \"emailSubject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject line of the email sent to recipients.\"\n    },\n    \"emailBlurb\": {\n      \"type\": \"string\",\n      \"description\": \"The body text of the email sent to recipients.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The envelope status. Set to \\\"sent\\\" to send the envelope immediately, or \\\"created\\\" to save as a draft.\"\n    },\n    \"templateId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of a template to use as the basis for the envelope. When specified, the template's documents, recipients, and tabs are merged with any specified in the\
  \ request.\"\n    },\n    \"templateRoles\": {\n      \"type\": \"array\",\n      \"description\": \"Template role assignments that map recipients to template roles when using a templateId.\"\n    },\n    \"documents\": {\n      \"type\": \"array\",\n      \"description\": \"The documents to include in the envelope.\"\n    },\n    \"compositeTemplates\": {\n      \"type\": \"array\",\n      \"description\": \"An array of composite template objects that combine server templates and inline templates for complex workflows.\"\n    },\n    \"brandId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the brand to apply to the envelope.\"\n    },\n    \"envelopeIdStamping\": {\n      \"type\": \"string\",\n      \"description\": \"When true, the envelope ID is stamped in the document margins.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-definition-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopeDefinition
---
