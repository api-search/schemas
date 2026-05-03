---
description: Represents a position in Workday, defining a specific role within an organization that can be filled by a worker. Positions are linked to job profiles and supervisory organizations.
layout: schema
name: Workday Position
properties_list:
- description: Workday ID of the position
  name: id
  type: string
- description: Display name of the position
  name: descriptor
  type: string
- description: Position ID code
  name: positionId
  type: string
- description: Whether the position is currently filled by a worker
  name: isFilled
  type: boolean
- description: ''
  name: worker
  type: object
- description: ''
  name: jobProfile
  type: object
- description: ''
  name: supervisoryOrganization
  type: object
- description: ''
  name: location
  type: object
- description: Date the position became or becomes available
  name: availableDate
  type: string
provider_name: Workday Integrations
provider_slug: workday-integrations
schema_file: json-schema/workday-integrations-position-schema.json
slug: workday-integrations-position
source_filename: workday-integrations-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-integrations/position.json\",\n  \"title\": \"Workday Position\",\n  \"description\": \"Represents a position in Workday, defining a specific role within an organization that can be filled by a worker. Positions are linked to job profiles and supervisory organizations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"descriptor\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Workday ID of the position\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the position\"\n    },\n    \"positionId\": {\n      \"type\": \"string\",\n      \"description\": \"Position ID code\"\n    },\n    \"isFilled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position is currently filled by a worker\"\n    },\n    \"worker\": {\n      \"\
  $ref\": \"#/$defs/Reference\"\n    },\n    \"jobProfile\": {\n      \"$ref\": \"#/$defs/Reference\"\n    },\n    \"supervisoryOrganization\": {\n      \"$ref\": \"#/$defs/Reference\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/Reference\"\n    },\n    \"availableDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the position became or becomes available\"\n    }\n  },\n  \"$defs\": {\n    \"Reference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a Workday business object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Workday ID of the referenced object\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the referenced object\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL for the referenced\
  \ resource\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/json-schema/workday-integrations-position-schema.json
tags:
- Cloud
- Enterprise Software
- ERP
- Finance
- HCM
- HR
- Integration
title: Workday Position
---
