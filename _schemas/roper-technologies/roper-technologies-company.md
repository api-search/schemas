---
description: Schema representing Roper Technologies' corporate structure, business segments, and portfolio of software subsidiaries.
layout: schema
name: Roper Technologies Company Profile
properties_list:
- description: Company name
  name: name
  type: string
- description: Stock ticker symbol
  name: ticker
  type: string
- description: Stock exchange
  name: exchange
  type: string
- description: Corporate website
  name: website
  type: string
- description: Corporate description
  name: description
  type: string
- description: Roper Technologies' three operating business segments
  name: segments
  type: array
provider_name: Roper Technologies
provider_slug: roper-technologies
schema_file: json-schema/roper-technologies-company-schema.json
slug: roper-technologies-company
source_filename: roper-technologies-company-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.ropertech.com/schemas/company.json\",\n  \"title\": \"Roper Technologies Company Profile\",\n  \"description\": \"Schema representing Roper Technologies' corporate structure, business segments, and portfolio of software subsidiaries.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"BusinessSegment\": {\n      \"type\": \"object\",\n      \"title\": \"BusinessSegment\",\n      \"description\": \"One of Roper Technologies' three operating segments\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Segment name\",\n          \"enum\": [\"Application Software\", \"Network Software\", \"Technology Enabled Products\"]\n        },\n        \"revenuePercentage\": {\n          \"type\": \"number\",\n          \"description\": \"Approximate percentage of total Roper Technologies revenue from this\
  \ segment\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"subsidiaries\": {\n          \"type\": \"array\",\n          \"description\": \"Subsidiary businesses within this segment\",\n          \"items\": { \"$ref\": \"#/$defs/Subsidiary\" }\n        }\n      }\n    },\n    \"Subsidiary\": {\n      \"type\": \"object\",\n      \"title\": \"Subsidiary\",\n      \"description\": \"A Roper Technologies portfolio company\",\n      \"required\": [\"name\", \"website\", \"verticalMarket\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Subsidiary company name\"\n        },\n        \"website\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Primary website URL\"\n        },\n        \"verticalMarket\": {\n          \"type\": \"string\",\n          \"description\": \"Industry vertical served by this subsidiary\"\n        },\n        \"description\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Description of the subsidiary's products and customers\"\n        },\n        \"apiDocumentation\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Developer/API documentation URL if available\"\n        },\n        \"revenueModel\": {\n          \"type\": \"string\",\n          \"description\": \"Primary revenue model\",\n          \"enum\": [\"SaaS\", \"Licensed\", \"Transactional\", \"Subscription\", \"Hardware + Software\"]\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"ticker\", \"segments\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Company name\",\n      \"const\": \"Roper Technologies\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Stock ticker symbol\",\n      \"const\": \"ROP\"\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Stock exchange\",\n      \"const\": \"NASDAQ\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Corporate website\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Corporate description\"\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Roper Technologies' three operating business segments\",\n      \"items\": { \"$ref\": \"#/$defs/BusinessSegment\" },\n      \"minItems\": 3,\n      \"maxItems\": 3\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/roper-technologies/refs/heads/main/json-schema/roper-technologies-company-schema.json
tags:
- B2B Software
- Enterprise Software
- Fortune 500
- Healthcare IT
- Insurance Technology
- Legal Technology
- SaaS
- Vertical Software
title: Roper Technologies Company Profile
---
