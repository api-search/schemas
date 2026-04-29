---
description: A business glossary containing terms and categories for data governance.
layout: schema
name: AtlasGlossary
properties_list:
- description: Unique identifier of the glossary.
  name: guid
  type: string
- description: Name of the glossary.
  name: name
  type: string
- description: Short description of the glossary.
  name: shortDescription
  type: string
- description: Long description of the glossary.
  name: longDescription
  type: string
- description: Language of the glossary.
  name: language
  type: string
- description: Number of terms in this glossary.
  name: termCount
  type: integer
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-glossary-schema.json
slug: atlas-atlas-glossary
source_filename: atlas-atlas-glossary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-glossary-schema.json\",\n  \"title\": \"AtlasGlossary\",\n  \"description\": \"A business glossary containing terms and categories for data governance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"guid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the glossary.\",\n      \"example\": \"glossary-guid-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the glossary.\",\n      \"example\": \"BusinessGlossary\"\n    },\n    \"shortDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the glossary.\",\n      \"example\": \"Enterprise business glossary for data governance\"\n    },\n    \"longDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Long description\
  \ of the glossary.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the glossary.\",\n      \"example\": \"en\"\n    },\n    \"termCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of terms in this glossary.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-glossary-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasGlossary
---
