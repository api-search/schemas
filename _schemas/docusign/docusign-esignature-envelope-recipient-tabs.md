---
description: Contains the tab collections for an envelope recipient, organized by tab type.
layout: schema
name: EnvelopeRecipientTabs
properties_list:
- description: Signature tabs requiring the recipient to sign.
  name: signHereTabs
  type: array
- description: Initial tabs requiring the recipient to initial.
  name: initialHereTabs
  type: array
- description: Date signed tabs auto-filled with the signing date.
  name: dateSignedTabs
  type: array
- description: Text input tabs for free-form text entry.
  name: textTabs
  type: array
- description: Full name tabs auto-filled with the signer name.
  name: fullNameTabs
  type: array
- description: Email tabs for email address input.
  name: emailTabs
  type: array
- description: Checkbox tabs for boolean selection.
  name: checkboxTabs
  type: array
- description: Radio button group tabs for single-choice selection.
  name: radioGroupTabs
  type: array
- description: List tabs for dropdown selection.
  name: listTabs
  type: array
- description: Number tabs for numeric input.
  name: numberTabs
  type: array
- description: Date tabs for date selection.
  name: dateTabs
  type: array
- description: Formula tabs for calculated values.
  name: formulaTabs
  type: array
- description: Note tabs for displaying read-only text.
  name: noteTabs
  type: array
- description: Approve tabs for document approval.
  name: approveTabs
  type: array
- description: Decline tabs for document rejection.
  name: declineTabs
  type: array
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-recipient-tabs-schema.json
slug: docusign-esignature-envelope-recipient-tabs
source_filename: docusign-esignature-envelope-recipient-tabs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopeRecipientTabs\",\n  \"type\": \"object\",\n  \"description\": \"Contains the tab collections for an envelope recipient, organized by tab type.\",\n  \"properties\": {\n    \"signHereTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Signature tabs requiring the recipient to sign.\"\n    },\n    \"initialHereTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Initial tabs requiring the recipient to initial.\"\n    },\n    \"dateSignedTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Date signed tabs auto-filled with the signing date.\"\n    },\n    \"textTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Text input tabs for free-form text entry.\"\n    },\n    \"fullNameTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Full name tabs auto-filled with the signer name.\"\n    },\n    \"emailTabs\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Email tabs for email address input.\"\n    },\n    \"checkboxTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Checkbox tabs for boolean selection.\"\n    },\n    \"radioGroupTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Radio button group tabs for single-choice selection.\"\n    },\n    \"listTabs\": {\n      \"type\": \"array\",\n      \"description\": \"List tabs for dropdown selection.\"\n    },\n    \"numberTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Number tabs for numeric input.\"\n    },\n    \"dateTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Date tabs for date selection.\"\n    },\n    \"formulaTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Formula tabs for calculated values.\"\n    },\n    \"noteTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Note tabs for displaying read-only text.\"\n    },\n    \"approveTabs\": {\n      \"type\": \"array\",\n\
  \      \"description\": \"Approve tabs for document approval.\"\n    },\n    \"declineTabs\": {\n      \"type\": \"array\",\n      \"description\": \"Decline tabs for document rejection.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-recipient-tabs-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopeRecipientTabs
---
