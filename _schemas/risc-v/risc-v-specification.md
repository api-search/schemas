---
description: A RISC-V International specification or technical standard
layout: schema
name: RISC-V Specification
properties_list:
- description: Specification identifier (e.g., riscv-isa-manual)
  name: id
  type: string
- description: Full specification title
  name: title
  type: string
- description: Specification category
  name: category
  type: string
- description: Ratification status
  name: status
  type: string
- description: Current version string
  name: version
  type: string
- description: GitHub repository URL
  name: githubRepository
  type: string
- description: PDF download URL for the specification
  name: pdfUrl
  type: string
- description: HTML version URL
  name: htmlUrl
  type: string
- description: RISC-V International working group responsible for the spec
  name: workingGroup
  type: string
- description: Related specification identifiers
  name: relatedSpecs
  type: array
- description: Known reference implementations
  name: implementations
  type: array
provider_name: RISC-V International
provider_slug: risc-v
schema_file: json-schema/risc-v-specification-schema.json
slug: risc-v-specification
source_filename: risc-v-specification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/risc-v/blob/main/json-schema/risc-v-specification-schema.json\",\n  \"title\": \"RISC-V Specification\",\n  \"description\": \"A RISC-V International specification or technical standard\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Specification identifier (e.g., riscv-isa-manual)\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Full specification title\",\n      \"example\": \"The RISC-V Instruction Set Manual, Volume I: Unprivileged ISA\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Specification category\",\n      \"enum\": [\"ISA Specification\", \"Non-ISA Specification\", \"Profile\", \"Extension\", \"Platform Specification\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Ratification\
  \ status\",\n      \"enum\": [\"Draft\", \"Development\", \"Stable\", \"Frozen\", \"Ratified\"]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Current version string\",\n      \"example\": \"20240411\"\n    },\n    \"githubRepository\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"GitHub repository URL\"\n    },\n    \"pdfUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"PDF download URL for the specification\"\n    },\n    \"htmlUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTML version URL\"\n    },\n    \"workingGroup\": {\n      \"type\": \"string\",\n      \"description\": \"RISC-V International working group responsible for the spec\"\n    },\n    \"relatedSpecs\": {\n      \"type\": \"array\",\n      \"description\": \"Related specification identifiers\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n  \
  \  },\n    \"implementations\": {\n      \"type\": \"array\",\n      \"description\": \"Known reference implementations\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"language\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"title\", \"category\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/risc-v/refs/heads/main/json-schema/risc-v-specification-schema.json
tags:
- C API
- Compiler
- Hardware
- Instruction Set Architecture
- Linux Foundation
- Open Hardware
- Open Source
- Processor
- RISC-V
- Simulator
title: RISC-V Specification
---
