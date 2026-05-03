---
description: Represents an employee or contingent worker within the Workday Human Capital Management system, including personal data, employment information, and organizational assignments.
layout: schema
name: Worker
properties_list:
- description: The unique Workday identifier for the worker
  name: id
  type: string
- description: The display name of the worker
  name: descriptor
  type: string
- description: The employee or contingent worker ID (e.g., EMP-001)
  name: workerID
  type: string
- description: The type of worker (Employee or Contingent Worker)
  name: workerType
  type: object
- description: The current business title of the worker
  name: businessTitle
  type: string
- description: The primary work email address
  name: primaryWorkEmail
  type: string
- description: The primary work phone number
  name: primaryWorkPhone
  type: string
- description: The supervisory organization to which the worker belongs
  name: supervisoryOrganization
  type: object
- description: The management level of the worker
  name: managementLevel
  type: object
- description: The work location of the worker
  name: location
  type: object
- description: The date the worker was hired
  name: hireDate
  type: string
- description: The date the worker was terminated, if applicable
  name: terminationDate
  type:
  - string
  - 'null'
- description: The position the worker currently holds
  name: position
  type: object
- description: The job profile associated with the worker's position
  name: jobProfile
  type: object
- description: Whether the worker is currently active
  name: isActive
  type: boolean
- description: URL to the worker's photo
  name: photo
  type: string
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-worker-schema.json
slug: workday-integration-worker
source_filename: workday-integration-worker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/worker\",\n  \"title\": \"Worker\",\n  \"description\": \"Represents an employee or contingent worker within the Workday Human Capital Management system, including personal data, employment information, and organizational assignments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the worker\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the worker\"\n    },\n    \"workerID\": {\n      \"type\": \"string\",\n      \"description\": \"The employee or contingent worker ID (e.g., EMP-001)\"\n    },\n    \"workerType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The type of worker (Employee or Contingent Worker)\"\n    },\n    \"businessTitle\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The current business title of the worker\"\n    },\n    \"primaryWorkEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The primary work email address\"\n    },\n    \"primaryWorkPhone\": {\n      \"type\": \"string\",\n      \"description\": \"The primary work phone number\"\n    },\n    \"supervisoryOrganization\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The supervisory organization to which the worker belongs\"\n    },\n    \"managementLevel\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The management level of the worker\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The work location of the worker\"\n    },\n    \"hireDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the worker was hired\"\n    },\n    \"terminationDate\": {\n      \"\
  type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The date the worker was terminated, if applicable\"\n    },\n    \"position\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The position the worker currently holds\"\n    },\n    \"jobProfile\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The job profile associated with the worker's position\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the worker is currently active\"\n    },\n    \"photo\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the worker's photo\"\n    }\n  },\n  \"required\": [\"id\", \"descriptor\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Workday resource\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The Workday ID of the referenced resource\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the referenced resource\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The API resource URL\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-worker-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Worker
---
