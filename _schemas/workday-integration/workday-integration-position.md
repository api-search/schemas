---
description: Represents a staffing position within the Workday system, defining a role within an organization that can be filled by a worker.
layout: schema
name: Position
properties_list:
- description: The unique Workday identifier for the position
  name: id
  type: string
- description: The display name of the position
  name: descriptor
  type: string
- description: The position reference ID
  name: positionID
  type: string
- description: The job profile associated with this position
  name: jobProfile
  type: object
- description: The supervisory organization this position belongs to
  name: supervisoryOrganization
  type: object
- description: The work location of the position
  name: location
  type: object
- description: Whether the position is currently filled by a worker
  name: isFilled
  type: boolean
- description: The worker currently filling this position
  name: worker
  type: object
- description: The date the position becomes available
  name: availableDate
  type:
  - string
  - 'null'
- description: The earliest date a hire can be made for this position
  name: earliestHireDate
  type:
  - string
  - 'null'
- description: The time type (Full Time, Part Time) for the position
  name: timeType
  type: object
- description: The worker type (Employee, Contingent Worker) for the position
  name: workerType
  type: object
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-position-schema.json
slug: workday-integration-position
source_filename: workday-integration-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/position\",\n  \"title\": \"Position\",\n  \"description\": \"Represents a staffing position within the Workday system, defining a role within an organization that can be filled by a worker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the position\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the position\"\n    },\n    \"positionID\": {\n      \"type\": \"string\",\n      \"description\": \"The position reference ID\"\n    },\n    \"jobProfile\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The job profile associated with this position\"\n    },\n    \"supervisoryOrganization\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The supervisory\
  \ organization this position belongs to\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The work location of the position\"\n    },\n    \"isFilled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position is currently filled by a worker\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker currently filling this position\"\n    },\n    \"availableDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The date the position becomes available\"\n    },\n    \"earliestHireDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The earliest date a hire can be made for this position\"\n    },\n    \"timeType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The time type (Full Time, Part Time) for the position\"\n    },\n  \
  \  \"workerType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker type (Employee, Contingent Worker) for the position\"\n    }\n  },\n  \"required\": [\"id\", \"descriptor\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-position-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Position
---
