---
description: PartMaster schema from 1Factory API
layout: schema
name: PartMaster
properties_list:
- description: ''
  name: ID
  type: object
- description: ''
  name: part_number
  type: object
- description: ''
  name: rev
  type: object
- description: Description of the part. (Optional).
  name: description
  type: string
- description: Status of Part Master entry.
  name: status
  type: string
- description: 'An alternative identifier used to identify a part, such as Drawing #, or customer / supplier part number.'
  name: alt_part_number
  type: string
- description: An alternate part revision, such as a drawing revision, or customer / supplier part revision.
  name: alt_rev
  type: string
- description: 'A second alternative identifier used to identify a part, such as Drawing #, or customer / supplier part number.'
  name: alt_part_number2
  type: string
- description: A second alternate part revision, such as a drawing revision, or customer / supplier part revision.
  name: alt_rev2
  type: string
- description: ''
  name: project_identifier
  type: object
- description: The number of plans this Part Master is associated with.
  name: plan_count
  type: number
- description: The number of NCRs this Part Master is associated with.
  name: ncr_count
  type: number
- description: Identify if the part is part of a regular part, tabulated part, or the parent tabulated part
  name: type
  type: string
- description: The part number of the parent part if this part is a Table of Size entry.
  name: parent_part_number
  type: string
- description: The part revision of the parent part if this part is a Table of Size entry.
  name: parent_rev
  type: string
- description: Cost of the part. (Optional).
  name: cost
  type: number
- description: Unit used for determine part cost. (Optional)
  name: unit
  type: string
- description: If true, indicates the part is setup as a library for a Spec Library.
  name: is_library
  type: boolean
- description: If true, indicates part is an assembly.
  name: is_assembly
  type: boolean
- description: If true, indicates part is an ITAR part with additional controls.
  name: is_itar
  type: boolean
- description: If true, indicates part has PPAP documents.
  name: has_ppap
  type: boolean
- description: ''
  name: component_parts
  type: array
- description: If true, indicates part is bought, rather than made. (Optional)
  name: is_buy
  type: boolean
- description: Detailed comments regarding the part. (Optional)
  name: comments
  type: string
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-part-master-schema.json
slug: 1factory-part-master
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-part-master-schema.json\",\n  \"title\": \"PartMaster\",\n  \"description\": \"PartMaster schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"$ref\": \"#/components/schemas/ID\"\n    },\n    \"part_number\": {\n      \"$ref\": \"#/components/schemas/part_number\"\n    },\n    \"rev\": {\n      \"$ref\": \"#/components/schemas/rev\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"Description of the part. (Optional).\",\n      \"example\": \"Three Lobe Shaft\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"nullable\": false,\n      \"enum\": [\n        \"Active\",\n        \"Inactive\"\n      ],\n      \"default\": \"Active\",\n      \"description\"\
  : \"Status of Part Master entry.\"\n    },\n    \"alt_part_number\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"An alternative identifier used to identify a part, such as Drawing #, or customer / supplier part number.\",\n      \"example\": \"DN-1234568\"\n    },\n    \"alt_rev\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"An alternate part revision, such as a drawing revision, or customer / supplier part revision.\",\n      \"example\": \"B\"\n    },\n    \"alt_part_number2\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"description\": \"A second alternative identifier used to identify a part, such as Drawing #, or customer / supplier part number.\",\n      \"example\": \"CN-1234569\"\n    },\n    \"alt_rev2\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255,\n      \"\
  description\": \"A second alternate part revision, such as a drawing revision, or customer / supplier part revision.\",\n      \"example\": \"C\"\n    },\n    \"project_identifier\": {\n      \"$ref\": \"#/components/schemas/project_identifier\"\n    },\n    \"plan_count\": {\n      \"type\": \"number\",\n      \"nullable\": false,\n      \"description\": \"The number of plans this Part Master is associated with.\",\n      \"example\": 2\n    },\n    \"ncr_count\": {\n      \"type\": \"number\",\n      \"nullable\": false,\n      \"description\": \"The number of NCRs this Part Master is associated with.\",\n      \"example\": 3\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Identify if the part is part of a regular part, tabulated part, or the parent tabulated part\",\n      \"enum\": [\n        \"Tabulated\",\n        \"ToS Entry\",\n        \"Standard\"\n      ]\n    },\n    \"parent_part_number\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The part number of the parent part if this part is a Table of Size entry.\"\n    },\n    \"parent_rev\": {\n      \"type\": \"string\",\n      \"description\": \"The part revision of the parent part if this part is a Table of Size entry.\"\n    },\n    \"cost\": {\n      \"type\": \"number\",\n      \"nullable\": true,\n      \"format\": \"double\",\n      \"description\": \"Cost of the part. (Optional).\",\n      \"example\": 3.5\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit used for determine part cost. (Optional)\",\n      \"example\": \"Each\"\n    },\n    \"is_library\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"If true, indicates the part is setup as a library for a Spec Library.\",\n      \"example\": false\n    },\n    \"is_assembly\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"If true, indicates part is an assembly.\"\n    },\n    \"is_itar\": {\n   \
  \   \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"If true, indicates part is an ITAR part with additional controls.\"\n    },\n    \"has_ppap\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"If true, indicates part has PPAP documents.\"\n    },\n    \"component_parts\": {\n      \"type\": \"array\",\n      \"minItems\": 0,\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AssemblyEntry\"\n      },\n      \"example\": []\n    },\n    \"is_buy\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"If true, indicates part is bought, rather than made. (Optional)\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 32000,\n      \"description\": \"Detailed comments regarding the part. (Optional)\",\n      \"example\": \"This is a brand new part that we are prototyping.\"\n    }\n  },\n  \"required\"\
  : [\n    \"part_number\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-part-master-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: PartMaster
---
