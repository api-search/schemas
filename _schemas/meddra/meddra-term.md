---
description: A term in the Medical Dictionary for Regulatory Activities (MedDRA) hierarchy
layout: schema
name: MedDRA Term
properties_list:
- description: MedDRA numeric term code (8 digits)
  name: code
  type: integer
- description: Official MedDRA term name
  name: termText
  type: string
- description: 'Hierarchy level: SOC=System Organ Class, HLGT=High Level Group Term, HLT=High Level Term, PT=Preferred Term, LLT=Lowest Level Term'
  name: level
  type: string
- description: Whether this term is current and not deprecated/retired
  name: current
  type: boolean
- description: Code of the primary System Organ Class for this term
  name: primarySOCCode
  type: integer
- description: Name of the primary System Organ Class
  name: primarySOCName
  type: string
- description: MedDRA dictionary version (e.g., 27.0)
  name: version
  type: string
- description: ISO 639-1 language code
  name: language
  type: string
- description: All SOC associations (a PT can belong to multiple SOCs)
  name: allSOCLinks
  type: array
provider_name: meddra
provider_slug: meddra
schema_file: json-schema/meddra-term-schema.json
slug: meddra-term
source_filename: meddra-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/json-schema/meddra-term-schema.json\",\n  \"title\": \"MedDRA Term\",\n  \"description\": \"A term in the Medical Dictionary for Regulatory Activities (MedDRA) hierarchy\",\n  \"type\": \"object\",\n  \"required\": [\"code\", \"termText\", \"level\", \"current\"],\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"MedDRA numeric term code (8 digits)\",\n      \"minimum\": 10000000,\n      \"maximum\": 99999999\n    },\n    \"termText\": {\n      \"type\": \"string\",\n      \"description\": \"Official MedDRA term name\",\n      \"maxLength\": 100\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"enum\": [\"SOC\", \"HLGT\", \"HLT\", \"PT\", \"LLT\"],\n      \"description\": \"Hierarchy level: SOC=System Organ Class, HLGT=High Level Group Term, HLT=High Level Term, PT=Preferred\
  \ Term, LLT=Lowest Level Term\"\n    },\n    \"current\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this term is current and not deprecated/retired\"\n    },\n    \"primarySOCCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Code of the primary System Organ Class for this term\"\n    },\n    \"primarySOCName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the primary System Organ Class\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"MedDRA dictionary version (e.g., 27.0)\",\n      \"pattern\": \"^[0-9]+\\\\.[0-9]+$\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 639-1 language code\",\n      \"default\": \"en\"\n    },\n    \"allSOCLinks\": {\n      \"type\": \"array\",\n      \"description\": \"All SOC associations (a PT can belong to multiple SOCs)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"socCode\", \"socName\"\
  , \"isPrimary\"],\n        \"properties\": {\n          \"socCode\": {\n            \"type\": \"integer\"\n          },\n          \"socName\": {\n            \"type\": \"string\"\n          },\n          \"isPrimary\": {\n            \"type\": \"boolean\",\n            \"description\": \"True if this is the primary SOC pathway\"\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"HierarchyLevels\": {\n      \"description\": \"MedDRA 5-level hierarchy\",\n      \"type\": \"string\",\n      \"enum\": [\"SOC\", \"HLGT\", \"HLT\", \"PT\", \"LLT\"],\n      \"x-description\": {\n        \"SOC\": \"System Organ Class — highest level, 27 classes (e.g., Hepatobiliary disorders)\",\n        \"HLGT\": \"High Level Group Term — groups multiple HLTs\",\n        \"HLT\": \"High Level Term — groups related PTs\",\n        \"PT\": \"Preferred Term — distinct medical concept for use in submissions\",\n        \"LLT\": \"Lowest Level Term — verbatim terms mapped to a PT\"\n      }\n  \
  \  }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/meddra/refs/heads/main/json-schema/meddra-term-schema.json
tags: []
title: MedDRA Term
---
