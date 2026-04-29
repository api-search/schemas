---
description: A US GAAP accounting standard entry from the FASB Accounting Standards Codification, representing a topic, subtopic, or accounting standards update.
layout: schema
name: GaapAccountingStandard
properties_list:
- description: FASB ASC topic or ASU identifier
  name: id
  type: string
- description: Title of the accounting standard or update
  name: title
  type: string
- description: FASB ASC topic number
  name: topic
  type: string
- description: Name of the ASC topic area
  name: topicName
  type: string
- description: Date the standard or update was issued
  name: issuedDate
  type: string
- description: Mandatory effective date for public business entities
  name: effectiveDate
  type: string
- description: Brief description of the standard's purpose and key requirements
  name: summary
  type: string
- description: Entities to which the standard applies
  name: applicability
  type: string
- description: URL to the standard in the FASB ASC or on fasb.org
  name: url
  type: string
- description: Other ASC topic numbers related to this standard
  name: relatedTopics
  type: array
provider_name: Accounting Standards
provider_slug: accounting-standards
schema_file: json-schema/gaap-accounting-standard-schema.json
slug: gaap-accounting-standard
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accounting-standards/refs/heads/main/json-schema/gaap-accounting-standard-schema.json\",\n  \"title\": \"GaapAccountingStandard\",\n  \"description\": \"A US GAAP accounting standard entry from the FASB Accounting Standards Codification, representing a topic, subtopic, or accounting standards update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"FASB ASC topic or ASU identifier\",\n      \"example\": \"ASU 2023-09\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the accounting standard or update\",\n      \"example\": \"Income Taxes (Topic 740): Improvements to Income Tax Disclosures\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"FASB ASC topic number\",\n      \"example\": \"740\"\n    },\n    \"\
  topicName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the ASC topic area\",\n      \"example\": \"Income Taxes\"\n    },\n    \"issuedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the standard or update was issued\",\n      \"example\": \"2023-12-14\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Mandatory effective date for public business entities\",\n      \"example\": \"2025-01-01\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Brief description of the standard's purpose and key requirements\"\n    },\n    \"applicability\": {\n      \"type\": \"string\",\n      \"description\": \"Entities to which the standard applies\",\n      \"enum\": [\"All entities\", \"Public business entities\", \"Nonpublic business entities\", \"Not-for-profit entities\"],\n      \"example\": \"All entities\"\n    },\n    \"\
  url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the standard in the FASB ASC or on fasb.org\",\n      \"example\": \"https://www.fasb.org/standards/accounting-standard-updates\"\n    },\n    \"relatedTopics\": {\n      \"type\": \"array\",\n      \"description\": \"Other ASC topic numbers related to this standard\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"946\", \"948\"]\n    }\n  },\n  \"required\": [\"id\", \"title\", \"topic\", \"issuedDate\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accounting-standards/refs/heads/main/json-schema/gaap-accounting-standard-schema.json
tags:
- Accounting Standards
- Finance
- GAAP
- IFRS
- XBRL
- Financial Reporting
- SEC
- FASB
title: GaapAccountingStandard
---
