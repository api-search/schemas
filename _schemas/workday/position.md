---
description: Represents a position in Workday. A position defines a role within a supervisory organization and can be filled by a worker.
layout: schema
name: Position
properties_list:
- description: The Workday ID of the position.
  name: id
  type: string
- description: A display descriptor for the position.
  name: descriptor
  type: string
- description: The position reference ID (e.g., P-00001).
  name: positionID
  type: string
- description: The job profile associated with this position.
  name: jobProfile
  type: object
- description: The name of the job profile.
  name: jobProfileName
  type: string
- description: The business title for this position.
  name: businessTitle
  type: string
- description: The supervisory organization this position belongs to.
  name: supervisoryOrganization
  type: object
- description: The worker currently filling this position, if any.
  name: worker
  type: object
- description: The time type for the position (e.g., Full Time, Part Time).
  name: positionTimeType
  type: object
- description: The worker type for this position (e.g., Employee, Contingent Worker).
  name: workerType
  type: object
- description: The worker sub-type for the position.
  name: workerSubType
  type: object
- description: The primary work location for the position.
  name: location
  type: object
- description: The compensation grade associated with this position.
  name: compensationGrade
  type: object
- description: The pay rate type (e.g., Salary, Hourly).
  name: payRateType
  type: object
- description: Whether the position is currently filled by a worker.
  name: isFilled
  type: boolean
- description: Whether the position is available for recruiting.
  name: isAvailableForRecruit
  type: boolean
- description: Whether the position has been closed.
  name: isClosed
  type: boolean
- description: Whether the position is frozen.
  name: isFrozen
  type: boolean
- description: The headcount for this position.
  name: headcountCount
  type: integer
- description: The date the position becomes available.
  name: availableDate
  type:
  - string
  - 'null'
- description: The earliest allowed hire date.
  name: earliestHireDate
  type:
  - string
  - 'null'
- description: A link to the full position resource.
  name: href
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/position.json
slug: position
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://workday.com/schemas/position.json\",\n  \"title\": \"Position\",\n  \"description\": \"Represents a position in Workday. A position defines a role within a supervisory organization and can be filled by a worker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the position.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the position.\"\n    },\n    \"positionID\": {\n      \"type\": \"string\",\n      \"description\": \"The position reference ID (e.g., P-00001).\"\n    },\n    \"jobProfile\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The job profile associated with this position.\"\n    },\n    \"jobProfileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job profile.\"\n\
  \    },\n    \"businessTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The business title for this position.\"\n    },\n    \"supervisoryOrganization\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The supervisory organization this position belongs to.\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker currently filling this position, if any.\"\n    },\n    \"positionTimeType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The time type for the position (e.g., Full Time, Part Time).\"\n    },\n    \"workerType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker type for this position (e.g., Employee, Contingent Worker).\"\n    },\n    \"workerSubType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker sub-type for the position.\"\n    },\n    \"location\": {\n      \"$ref\"\
  : \"#/$defs/ResourceReference\",\n      \"description\": \"The primary work location for the position.\"\n    },\n    \"compensationGrade\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The compensation grade associated with this position.\"\n    },\n    \"payRateType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The pay rate type (e.g., Salary, Hourly).\"\n    },\n    \"isFilled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position is currently filled by a worker.\"\n    },\n    \"isAvailableForRecruit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position is available for recruiting.\"\n    },\n    \"isClosed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position has been closed.\"\n    },\n    \"isFrozen\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position is frozen.\"\n    },\n    \"headcountCount\": {\n     \
  \ \"type\": \"integer\",\n      \"description\": \"The headcount for this position.\"\n    },\n    \"availableDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The date the position becomes available.\"\n    },\n    \"earliestHireDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The earliest allowed hire date.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A link to the full position resource.\"\n    }\n  },\n  \"required\": [\"id\", \"descriptor\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Workday resource.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Workday ID of the referenced resource.\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n     \
  \     \"description\": \"A display descriptor for the referenced resource.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A link to the referenced resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/position.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Position
---
