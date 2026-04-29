---
description: ''
layout: schema
name: sharesOutstandingResponseObject
properties_list:
- description: Security-level FactSet Permanent Identifier associated with the identifier.
  name: fsymId
  type: string
- description: Date of the record in YYYY-MM-DD format.
  name: date
  type: string
- description: Unique Identifier for each document or filing which contains the outstanding shares position.
  name: documentId
  type: string
- description: FactSet Security Permanent Identifier that was used for the request.
  name: requestId
  type: string
- description: Reporting date of the position.
  name: reportDate
  type: string
- description: Exact date that results have been communicated to the market.
  name: publicationDate
  type: string
- description: The company's fiscal year corresponding to the report.
  name: fiscalYear
  type: integer
- description: Textual description of the reporting period.
  name: reportingPeriodDescription
  type: string
- description: 'Code representing the unique reporting period. Options are as follows: - 1 - 1st Quarter - 2 - 2nd Quarter - 3 - 3rd Quarter - 4 - 4th Quarter - 6 - Mid-Year'
  name: reportingPeriod
  type: integer
- description: Different stock types based on the rights and benefits from ownership.
  name: description
  type: string
- description: Different stock types based on the rights and benefits from ownership for the ADR.
  name: adrDescription
  type: string
- description: Number of common or ordinary shares that are equivalent to one American Depositary Receipt (ADR).
  name: adrRatio
  type: number
- description: Unique FactSet generated identifier assigned to a security, representing the ADR security.
  name: adrFsymId
  type: string
- description: Number of shares outstanding as of `date`.
  name: totalOutstanding
  type: number
- description: Number of shares outstanding for the ADR as of `date`.
  name: adrTotalOutstanding
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-prices-shares-outstanding-response-object-schema.json
slug: factset-global-prices-shares-outstanding-response-object
source_filename: factset-global-prices-shares-outstanding-response-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"sharesOutstandingResponseObject\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Security-level FactSet Permanent Identifier associated with the identifier.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the record in YYYY-MM-DD format.\"\n    },\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Identifier for each document or filing which contains the outstanding shares position.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Permanent Identifier that was used for the request.\"\n    },\n    \"reportDate\": {\n      \"type\": \"string\",\n      \"description\": \"Reporting date of the position.\"\n    },\n    \"publicationDate\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Exact date that results have been communicated to the market.\"\n    },\n    \"fiscalYear\": {\n      \"type\": \"integer\",\n      \"description\": \"The company's fiscal year corresponding to the report.\"\n    },\n    \"reportingPeriodDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Textual description of the reporting period.\"\n    },\n    \"reportingPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Code representing the unique reporting period. Options are as follows:\\n- 1 - 1st Quarter\\n- 2 - 2nd Quarter\\n- 3 - 3rd Quarter\\n- 4 - 4th Quarter\\n- 6 - Mid-Year\\n\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Different stock types based on the rights and benefits from ownership.\"\n    },\n    \"adrDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Different stock types based on the rights and benefits from ownership for the ADR.\"\n    },\n    \"adrRatio\": {\n      \"type\"\
  : \"number\",\n      \"description\": \"Number of common or ordinary shares that are equivalent to one American Depositary Receipt (ADR).\"\n    },\n    \"adrFsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique FactSet generated identifier assigned to a security, representing the ADR security.\"\n    },\n    \"totalOutstanding\": {\n      \"type\": \"number\",\n      \"description\": \"Number of shares outstanding as of `date`.\"\n    },\n    \"adrTotalOutstanding\": {\n      \"type\": \"number\",\n      \"description\": \"Number of shares outstanding for the ADR as of `date`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-shares-outstanding-response-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: sharesOutstandingResponseObject
---
