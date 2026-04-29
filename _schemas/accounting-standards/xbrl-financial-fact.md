---
description: A single XBRL financial fact from an SEC EDGAR filing, representing one tagged data point from a company's financial statements.
layout: schema
name: XbrlFinancialFact
properties_list:
- description: The SEC Central Index Key (CIK) of the filing entity, zero-padded to 10 digits
  name: cik
  type: string
- description: The XBRL taxonomy namespace prefix used for this fact
  name: taxonomy
  type: string
- description: The XBRL taxonomy element (tag) name for this fact
  name: concept
  type: string
- description: Human-readable label for the concept
  name: label
  type: string
- description: Definition of the taxonomy concept
  name: description
  type: string
- description: Legal name of the filing entity
  name: entityName
  type: string
- description: Array of unit groupings for this fact
  name: units
  type: array
provider_name: Accounting Standards
provider_slug: accounting-standards
schema_file: json-schema/xbrl-financial-fact-schema.json
slug: xbrl-financial-fact
source_filename: xbrl-financial-fact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accounting-standards/refs/heads/main/json-schema/xbrl-financial-fact-schema.json\",\n  \"title\": \"XbrlFinancialFact\",\n  \"description\": \"A single XBRL financial fact from an SEC EDGAR filing, representing one tagged data point from a company's financial statements.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cik\": {\n      \"type\": \"string\",\n      \"description\": \"The SEC Central Index Key (CIK) of the filing entity, zero-padded to 10 digits\",\n      \"example\": \"0000320193\",\n      \"pattern\": \"^[0-9]{10}$\"\n    },\n    \"taxonomy\": {\n      \"type\": \"string\",\n      \"description\": \"The XBRL taxonomy namespace prefix used for this fact\",\n      \"enum\": [\"us-gaap\", \"ifrs-full\", \"dei\", \"srt\"],\n      \"example\": \"us-gaap\"\n    },\n    \"concept\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The XBRL taxonomy element (tag) name for this fact\",\n      \"example\": \"Assets\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label for the concept\",\n      \"example\": \"Assets\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Definition of the taxonomy concept\"\n    },\n    \"entityName\": {\n      \"type\": \"string\",\n      \"description\": \"Legal name of the filing entity\",\n      \"example\": \"Apple Inc.\"\n    },\n    \"units\": {\n      \"type\": \"array\",\n      \"description\": \"Array of unit groupings for this fact\",\n      \"items\": {\n        \"$ref\": \"#/$defs/UnitFacts\"\n      }\n    }\n  },\n  \"required\": [\"cik\", \"taxonomy\", \"concept\"],\n  \"$defs\": {\n    \"UnitFacts\": {\n      \"type\": \"object\",\n      \"description\": \"Facts reported in a specific unit of measure\",\n      \"properties\": {\n        \"unit\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Unit of measure (e.g. USD, shares)\",\n          \"example\": \"USD\"\n        },\n        \"facts\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Fact\"\n          }\n        }\n      },\n      \"required\": [\"unit\", \"facts\"]\n    },\n    \"Fact\": {\n      \"type\": \"object\",\n      \"description\": \"A single data point from a specific filing period\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Start date for period-based facts (e.g. income statement items)\",\n          \"example\": \"2024-01-01\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"End date for the reporting period\",\n          \"example\": \"2024-12-31\"\n        },\n        \"val\": {\n          \"type\": \"number\",\n          \"description\": \"The numeric\
  \ value of the fact\",\n          \"example\": 364980000000\n        },\n        \"accn\": {\n          \"type\": \"string\",\n          \"description\": \"SEC accession number of the filing containing this fact\",\n          \"example\": \"0000320193-25-000001\"\n        },\n        \"fy\": {\n          \"type\": \"integer\",\n          \"description\": \"Fiscal year of the filing\",\n          \"example\": 2024\n        },\n        \"fp\": {\n          \"type\": \"string\",\n          \"description\": \"Fiscal period (Q1, Q2, Q3, Q4, FY, H1, H2)\",\n          \"enum\": [\"Q1\", \"Q2\", \"Q3\", \"Q4\", \"FY\", \"H1\", \"H2\"],\n          \"example\": \"FY\"\n        },\n        \"form\": {\n          \"type\": \"string\",\n          \"description\": \"SEC form type for the filing\",\n          \"example\": \"10-K\"\n        },\n        \"filed\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date the filing was submitted to SEC EDGAR\"\
  ,\n          \"example\": \"2025-02-01\"\n        },\n        \"frame\": {\n          \"type\": \"string\",\n          \"description\": \"XBRL frame identifier for period/concept aggregation\",\n          \"example\": \"CY2024Q4I\"\n        }\n      },\n      \"required\": [\"end\", \"val\", \"form\", \"filed\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accounting-standards/refs/heads/main/json-schema/xbrl-financial-fact-schema.json
tags:
- Accounting Standards
- Finance
- GAAP
- IFRS
- XBRL
- Financial Reporting
- SEC
- FASB
title: XbrlFinancialFact
---
