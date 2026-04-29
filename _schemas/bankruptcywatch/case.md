---
description: A US bankruptcy court case
layout: schema
name: Case
properties_list:
- description: BankruptcyWatch internal case ID
  name: caseId
  type: string
- description: PACER case number
  name: caseNumber
  type: string
- description: Name of the debtor
  name: debtorName
  type: string
- description: Bankruptcy chapter (7, 11, 13, etc.)
  name: chapter
  type: string
- description: Bankruptcy court district code
  name: district
  type: string
- description: Date the case was filed
  name: dateFiled
  type: string
- description: Current case status
  name: status
  type: string
- description: Assigned bankruptcy judge
  name: judge
  type: string
- description: Appointed trustee name
  name: trustee
  type: string
- description: Asset amount range
  name: assets
  type: string
- description: Liability amount range
  name: liabilities
  type: string
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/case-schema.json
slug: case
source_filename: case-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/case-schema.json\",\n  \"title\": \"Case\",\n  \"type\": \"object\",\n  \"description\": \"A US bankruptcy court case\",\n  \"properties\": {\n    \"caseId\": {\n      \"type\": \"string\",\n      \"description\": \"BankruptcyWatch internal case ID\"\n    },\n    \"caseNumber\": {\n      \"type\": \"string\",\n      \"description\": \"PACER case number\"\n    },\n    \"debtorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the debtor\"\n    },\n    \"chapter\": {\n      \"type\": \"string\",\n      \"description\": \"Bankruptcy chapter (7, 11, 13, etc.)\"\n    },\n    \"district\": {\n      \"type\": \"string\",\n      \"description\": \"Bankruptcy court district code\"\n    },\n    \"dateFiled\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the case was filed\"\n\
  \    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current case status\",\n      \"enum\": [\n        \"open\",\n        \"closed\",\n        \"discharged\",\n        \"dismissed\",\n        \"converted\"\n      ]\n    },\n    \"judge\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned bankruptcy judge\"\n    },\n    \"trustee\": {\n      \"type\": \"string\",\n      \"description\": \"Appointed trustee name\"\n    },\n    \"assets\": {\n      \"type\": \"string\",\n      \"description\": \"Asset amount range\"\n    },\n    \"liabilities\": {\n      \"type\": \"string\",\n      \"description\": \"Liability amount range\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/case-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: Case
---
