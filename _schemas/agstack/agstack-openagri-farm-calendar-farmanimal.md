---
description: ''
layout: schema
name: FarmAnimal
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: nationalID
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: hasAgriParcel
  type: string
- description: ''
  name: sex
  type: object
- description: ''
  name: isCastrated
  type: boolean
- description: ''
  name: species
  type: string
- description: ''
  name: breed
  type: string
- description: ''
  name: birthdate
  type: string
- description: ''
  name: isMemberOfAnimalGroup
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: invalidatedAtTime
  type: string
- description: ''
  name: dateCreated
  type: string
- description: ''
  name: dateModified
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-farmanimal-schema.json
slug: agstack-openagri-farm-calendar-farmanimal
source_filename: agstack-openagri-farm-calendar-farmanimal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/FarmAnimal.json\",\n  \"title\": \"FarmAnimal\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"nationalID\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 100\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"hasAgriParcel\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"sex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SexEnum\"\n        }\n      ],\n      \"minimum\": -2147483648,\n      \"maximum\": 2147483647\n    },\n    \"isCastrated\": {\n      \"type\": \"boolean\"\n    },\n    \"species\": {\n      \"type\": \"string\",\n      \"maxLength\": 255\n\
  \    },\n    \"breed\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255\n    },\n    \"birthdate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"isMemberOfAnimalGroup\": {\n      \"$ref\": \"#/components/schemas/FarmAnimalGroupSerializerField\"\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusEnum\"\n        }\n      ],\n      \"minimum\": -2147483648,\n      \"maximum\": 2147483647\n    },\n    \"invalidatedAtTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"birthdate\",\n    \"dateCreated\",\n    \"dateModified\",\n    \"hasAgriParcel\"\
  ,\n    \"id\",\n    \"invalidatedAtTime\",\n    \"species\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-farmanimal-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: FarmAnimal
---
