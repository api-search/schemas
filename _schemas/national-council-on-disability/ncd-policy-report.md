---
description: A policy report published by the National Council on Disability containing recommendations to the President, Congress, or federal agencies.
layout: schema
name: NCD Policy Report
properties_list:
- description: Full title of the NCD policy report
  name: title
  type: string
- description: Date the report was published
  name: publicationDate
  type: string
- description: Primary policy area covered by the report
  name: policyArea
  type: string
- description: Executive summary or abstract of the report
  name: summary
  type: string
- description: List of policy recommendations made in the report
  name: recommendations
  type: array
- description: URL to download the full report
  name: documentURL
  type: string
- description: Document file format
  name: format
  type: string
- description: Publication year
  name: year
  type: integer
provider_name: National Council on Disability
provider_slug: national-council-on-disability
schema_file: json-schema/ncd-policy-report-schema.json
slug: ncd-policy-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.ncd.gov/schemas/policy-report\",\n  \"title\": \"NCD Policy Report\",\n  \"description\": \"A policy report published by the National Council on Disability containing recommendations to the President, Congress, or federal agencies.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"title\",\n    \"publicationDate\",\n    \"policyArea\"\n  ],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Full title of the NCD policy report\"\n    },\n    \"publicationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the report was published\"\n    },\n    \"policyArea\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Civil Rights\",\n        \"Healthcare\",\n        \"Transportation\",\n        \"Employment\",\n        \"Housing\",\n        \"Financial Assistance\",\n        \"Emergency\
  \ Management\",\n        \"Education\",\n        \"Technology\",\n        \"International\"\n      ],\n      \"description\": \"Primary policy area covered by the report\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Executive summary or abstract of the report\"\n    },\n    \"recommendations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of policy recommendations made in the report\"\n    },\n    \"documentURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the full report\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PDF\",\n        \"HTML\",\n        \"Word\"\n      ],\n      \"description\": \"Document file format\"\n    },\n    \"year\": {\n      \"type\": \"integer\",\n      \"minimum\": 1984,\n      \"description\": \"Publication year\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/national-council-on-disability/refs/heads/main/json-schema/ncd-policy-report-schema.json
tags:
- Disability
- Federal Government
- Policy
- Civil Rights
- Healthcare
- Independent Agency
title: NCD Policy Report
---
