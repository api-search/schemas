---
description: Schema for a regulatory document such as a proposed rule, final rule, notice, or guidance document as returned by the Federal Register API or Regulations.gov API.
layout: schema
name: Regulatory Document
properties_list:
- description: Unique identifier for the regulatory document.
  name: documentId
  type: string
- description: Associated regulatory docket identifier.
  name: docketId
  type: string
- description: Official title of the regulatory document.
  name: title
  type: string
- description: Type of regulatory document.
  name: type
  type: string
- description: Identifier of the issuing agency (e.g., 'EPA', 'HHS', 'SEC').
  name: agencyId
  type: string
- description: Full name of the issuing agency.
  name: agencyName
  type: string
- description: Date the document was published in the Federal Register.
  name: publicationDate
  type: string
- description: Date the rule becomes effective (for Final Rules).
  name: effectiveDate
  type: string
- description: Deadline for public comments (for Proposed Rules).
  name: commentDeadline
  type: string
- description: Number of public comments received.
  name: commentCount
  type: integer
- description: Whether the document is currently open for public comment.
  name: openForComment
  type: boolean
- description: Code of Federal Regulations citations affected by this document.
  name: cfrCitations
  type: array
- description: Federal Register document number.
  name: federalRegisterNumber
  type: string
- description: Brief abstract or summary of the regulatory document.
  name: abstractText
  type: string
- description: URL to the full text of the document.
  name: fullTextUrl
  type: string
- description: URL to the PDF version of the document.
  name: pdfUrl
  type: string
- description: Subject matter topics covered by this document.
  name: topics
  type: array
- description: Regulation Identifier Number from the Unified Agenda.
  name: rin
  type: string
provider_name: Regulation
provider_slug: regulation
schema_file: json-schema/regulation-document-schema.json
slug: regulation-document
source_filename: regulation-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/regulation/json-schema/regulation-document-schema.json\",\n  \"title\": \"Regulatory Document\",\n  \"description\": \"Schema for a regulatory document such as a proposed rule, final rule, notice, or guidance document as returned by the Federal Register API or Regulations.gov API.\",\n  \"type\": \"object\",\n  \"required\": [\"documentId\", \"title\", \"type\", \"agencyId\", \"publicationDate\"],\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the regulatory document.\"\n    },\n    \"docketId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated regulatory docket identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Official title of the regulatory document.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Type of regulatory document.\",\n      \"enum\": [\"Proposed Rule\", \"Final Rule\", \"Notice\", \"Rule\", \"Presidential Document\", \"Correction\", \"Sunshine Act Meeting\", \"Executive Order\"]\n    },\n    \"agencyId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the issuing agency (e.g., 'EPA', 'HHS', 'SEC').\"\n    },\n    \"agencyName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the issuing agency.\"\n    },\n    \"publicationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the document was published in the Federal Register.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the rule becomes effective (for Final Rules).\"\n    },\n    \"commentDeadline\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Deadline for public comments (for Proposed Rules).\"\n    },\n\
  \    \"commentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of public comments received.\"\n    },\n    \"openForComment\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the document is currently open for public comment.\"\n    },\n    \"cfrCitations\": {\n      \"type\": \"array\",\n      \"description\": \"Code of Federal Regulations citations affected by this document.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"CFR citation (e.g., '40 CFR Part 122').\"\n      }\n    },\n    \"federalRegisterNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Federal Register document number.\"\n    },\n    \"abstractText\": {\n      \"type\": \"string\",\n      \"description\": \"Brief abstract or summary of the regulatory document.\"\n    },\n    \"fullTextUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the full text of the document.\"\n    },\n  \
  \  \"pdfUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the PDF version of the document.\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Subject matter topics covered by this document.\"\n    },\n    \"rin\": {\n      \"type\": \"string\",\n      \"description\": \"Regulation Identifier Number from the Unified Agenda.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/regulation/refs/heads/main/json-schema/regulation-document-schema.json
tags:
- Compliance
- Governance
- Government
- Legal
- Policy
- Regulation
- Regulatory Change
- Risk Management
title: Regulatory Document
---
