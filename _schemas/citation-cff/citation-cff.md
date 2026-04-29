---
description: A pragmatic JSON Schema profile of the Citation File Format 1.2.0 capturing the most commonly used fields. The authoritative schema is published at https://github.com/citation-file-format/citation-file-format.
layout: schema
name: Citation File Format (CFF) - Subset Profile
properties_list:
- description: The version of the CFF schema this file complies with.
  name: cff-version
  type: string
- description: Human-readable message instructing how to cite the software.
  name: message
  type: string
- description: The name of the software or dataset being cited.
  name: title
  type: string
- description: The released version being cited.
  name: version
  type: string
- description: DOI of the software or dataset.
  name: doi
  type: string
- description: ISO 8601 date the version was released.
  name: date-released
  type: string
- description: SPDX license identifier.
  name: license
  type: string
- description: URL of the source code repository.
  name: repository-code
  type: string
- description: URL of the software project.
  name: url
  type: string
- description: Short description of the software.
  name: abstract
  type: string
- description: Keywords describing the software.
  name: keywords
  type: array
- description: ''
  name: authors
  type: array
- description: ''
  name: preferred-citation
  type: object
- description: ''
  name: references
  type: array
- description: ''
  name: identifiers
  type: array
- description: ''
  name: type
  type: string
provider_name: Citation File Format
provider_slug: citation-cff
schema_file: json-schema/citation-cff-schema.json
slug: citation-cff
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/citation-cff/main/json-schema/citation-cff-schema.json\",\n  \"title\": \"Citation File Format (CFF) - Subset Profile\",\n  \"description\": \"A pragmatic JSON Schema profile of the Citation File Format 1.2.0 capturing the most commonly used fields. The authoritative schema is published at https://github.com/citation-file-format/citation-file-format.\",\n  \"type\": \"object\",\n  \"required\": [\"cff-version\", \"message\", \"authors\", \"title\"],\n  \"properties\": {\n    \"cff-version\": {\n      \"type\": \"string\",\n      \"pattern\": \"^1\\\\.[0-9]+\\\\.[0-9]+$\",\n      \"description\": \"The version of the CFF schema this file complies with.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"Human-readable message instructing how to cite the software.\"\n    },\n    \"title\":\
  \ {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"The name of the software or dataset being cited.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The released version being cited.\"\n    },\n    \"doi\": {\n      \"type\": \"string\",\n      \"pattern\": \"^10\\\\.[0-9]{4,}/.+\",\n      \"description\": \"DOI of the software or dataset.\"\n    },\n    \"date-released\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"ISO 8601 date the version was released.\"\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"description\": \"SPDX license identifier.\"\n    },\n    \"repository-code\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the source code repository.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the software project.\"\n    },\n    \"abstract\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Short description of the software.\"\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\"},\n      \"description\": \"Keywords describing the software.\"\n    },\n    \"authors\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\"$ref\": \"#/$defs/Author\"}\n    },\n    \"preferred-citation\": {\"$ref\": \"#/$defs/Reference\"},\n    \"references\": {\n      \"type\": \"array\",\n      \"items\": {\"$ref\": \"#/$defs/Reference\"}\n    },\n    \"identifiers\": {\n      \"type\": \"array\",\n      \"items\": {\"$ref\": \"#/$defs/Identifier\"}\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"software\", \"dataset\"]\n    }\n  },\n  \"$defs\": {\n    \"Author\": {\n      \"type\": \"object\",\n      \"oneOf\": [\n        {\"required\": [\"family-names\"]},\n        {\"required\": [\"name\"]}\n      ],\n      \"properties\": {\n        \"family-names\"\
  : {\"type\": \"string\"},\n        \"given-names\": {\"type\": \"string\"},\n        \"name\": {\"type\": \"string\"},\n        \"name-particle\": {\"type\": \"string\"},\n        \"name-suffix\": {\"type\": \"string\"},\n        \"alias\": {\"type\": \"string\"},\n        \"affiliation\": {\"type\": \"string\"},\n        \"email\": {\"type\": \"string\", \"format\": \"email\"},\n        \"orcid\": {\"type\": \"string\", \"pattern\": \"^https://orcid\\\\.org/[0-9]{4}-[0-9]{4}-[0-9]{4}-[0-9X]{4}$\"}\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\"type\": \"string\"},\n        \"title\": {\"type\": \"string\"},\n        \"authors\": {\"type\": \"array\", \"items\": {\"$ref\": \"#/$defs/Author\"}},\n        \"year\": {\"type\": \"integer\"},\n        \"month\": {\"type\": \"integer\"},\n        \"publisher\": {\"type\": \"object\"},\n        \"doi\": {\"type\": \"string\"},\n        \"url\"\
  : {\"type\": \"string\", \"format\": \"uri\"},\n        \"journal\": {\"type\": \"string\"},\n        \"volume\": {\"type\": \"integer\"},\n        \"issue\": {\"type\": \"string\"},\n        \"start\": {\"type\": \"integer\"},\n        \"end\": {\"type\": \"integer\"}\n      }\n    },\n    \"Identifier\": {\n      \"type\": \"object\",\n      \"required\": [\"type\", \"value\"],\n      \"properties\": {\n        \"type\": {\"type\": \"string\", \"enum\": [\"doi\", \"url\", \"swh\", \"other\"]},\n        \"value\": {\"type\": \"string\"},\n        \"description\": {\"type\": \"string\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citation-cff/refs/heads/main/json-schema/citation-cff-schema.json
tags:
- Academic
- Citation
- Metadata
- Open Standard
- Repository
- Research
- Software
- YAML
title: Citation File Format (CFF) - Subset Profile
---
