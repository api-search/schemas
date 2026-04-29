---
description: JSON Schema for an Autodesk Construction Cloud (ACC) project.
layout: schema
name: Autodesk Construction Cloud Project
properties_list:
- description: Unique ACC project identifier
  name: id
  type: string
- description: Parent account identifier
  name: accountId
  type: string
- description: Project name
  name: name
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: projectValue
  type: object
- description: ''
  name: status
  type: string
- description: ''
  name: jobNumber
  type: string
- description: ''
  name: addressLine1
  type: string
- description: ''
  name: addressLine2
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: stateOrProvince
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: timezone
  type: string
- description: ''
  name: language
  type: string
- description: Type of construction (e.g., New Construction, Renovation, Infrastructure)
  name: constructionType
  type: string
- description: Project delivery method (e.g., Design-Build, Design-Bid-Build, CM at Risk)
  name: deliveryMethod
  type: string
- description: Contract type (e.g., Fixed Price, Cost Plus, Unit Price)
  name: contractType
  type: string
- description: Current project phase
  name: currentPhase
  type: string
- description: ''
  name: businessUnitsId
  type: string
- description: ''
  name: imageUrl
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Autodesk Construction Cloud
provider_slug: autodesk-construction-cloud
schema_file: json-schema/acc-project-schema.json
slug: acc-project
source_filename: acc-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/json-schema/acc-project-schema.json\",\n  \"title\": \"Autodesk Construction Cloud Project\",\n  \"description\": \"JSON Schema for an Autodesk Construction Cloud (ACC) project.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ACC project identifier\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent account identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Project name\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"projectValue\": {\n      \"type\": \"object\"\
  ,\n      \"properties\": {\n        \"value\": {\"type\": \"number\", \"minimum\": 0},\n        \"currency\": {\"type\": \"string\", \"pattern\": \"^[A-Z]{3}$\"}\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"suspended\"]\n    },\n    \"jobNumber\": {\n      \"type\": \"string\"\n    },\n    \"addressLine1\": {\"type\": \"string\"},\n    \"addressLine2\": {\"type\": \"string\"},\n    \"city\": {\"type\": \"string\"},\n    \"stateOrProvince\": {\"type\": \"string\"},\n    \"postalCode\": {\"type\": \"string\"},\n    \"country\": {\"type\": \"string\"},\n    \"timezone\": {\"type\": \"string\"},\n    \"language\": {\"type\": \"string\"},\n    \"constructionType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of construction (e.g., New Construction, Renovation, Infrastructure)\"\n    },\n    \"deliveryMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Project delivery method (e.g., Design-Build,\
  \ Design-Bid-Build, CM at Risk)\"\n    },\n    \"contractType\": {\n      \"type\": \"string\",\n      \"description\": \"Contract type (e.g., Fixed Price, Cost Plus, Unit Price)\"\n    },\n    \"currentPhase\": {\n      \"type\": \"string\",\n      \"description\": \"Current project phase\"\n    },\n    \"businessUnitsId\": {\n      \"type\": \"string\"\n    },\n    \"imageUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/json-schema/acc-project-schema.json
tags:
- Construction
- BIM
- Project Management
- AEC
- CAD
- Architecture
- Engineering
- Field Management
title: Autodesk Construction Cloud Project
---
