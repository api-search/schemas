---
description: Schema for a FHIR R4 Bundle returned by the Community Health Systems Patient Access and Provider Directory APIs.
layout: schema
name: CHS FHIR Bundle
properties_list:
- description: ''
  name: resourceType
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: total
  type: integer
- description: ''
  name: link
  type: array
- description: ''
  name: entry
  type: array
provider_name: Community Health Systems
provider_slug: community-health-systems
schema_file: json-schema/chs-fhir-bundle-schema.json
slug: chs-fhir-bundle
source_filename: chs-fhir-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/community-health-systems/refs/heads/main/json-schema/chs-fhir-bundle-schema.json\",\n  \"title\": \"CHS FHIR Bundle\",\n  \"description\": \"Schema for a FHIR R4 Bundle returned by the Community Health Systems Patient Access and Provider Directory APIs.\",\n  \"type\": \"object\",\n  \"required\": [\"resourceType\"],\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"const\": \"Bundle\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"searchset\", \"collection\", \"history\", \"transaction\", \"transaction-response\", \"batch\", \"batch-response\", \"document\", \"message\"]\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"link\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\"\
  : \"object\",\n        \"properties\": {\n          \"relation\": { \"type\": \"string\" },\n          \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n        }\n      }\n    },\n    \"entry\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fullUrl\": { \"type\": \"string\", \"format\": \"uri\" },\n          \"resource\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"resourceType\": {\n                \"type\": \"string\",\n                \"enum\": [\"Patient\", \"ExplanationOfBenefit\", \"MedicationKnowledge\", \"Practitioner\", \"Organization\", \"Location\", \"Coverage\", \"Encounter\", \"Observation\"]\n              },\n              \"id\": { \"type\": \"string\" }\n            },\n            \"required\": [\"resourceType\"]\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/community-health-systems/refs/heads/main/json-schema/chs-fhir-bundle-schema.json
tags:
- CMS-9115-F
- FHIR
- Healthcare
- Hospitals
- Interoperability
- Patient Access
- Provider Directory
- SMART-on-FHIR
title: CHS FHIR Bundle
---
