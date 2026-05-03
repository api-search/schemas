---
description: A worker record in Oracle Fusion Cloud HCM representing an employee or contingent worker, including person details, employment information, and work assignments.
layout: schema
name: Oracle Fusion Cloud Worker
properties_list:
- description: Unique system-generated person identifier
  name: PersonId
  type: integer
- description: Unique person number assigned to the worker
  name: PersonNumber
  type: string
- description: Worker first name
  name: FirstName
  type: string
- description: Worker last name
  name: LastName
  type: string
- description: Worker middle name
  name: MiddleName
  type: string
- description: Full formatted display name
  name: DisplayName
  type: string
- description: Worker date of birth
  name: DateOfBirth
  type: string
- description: Primary work email address
  name: WorkEmail
  type: string
- description: Primary work phone number
  name: WorkPhoneNumber
  type: string
- description: Original hire date
  name: HireDate
  type: string
- description: Effective start date of the current record
  name: EffectiveStartDate
  type: string
- description: Classification of the worker relationship
  name: WorkerType
  type: string
- description: Detailed person type classification
  name: PersonType
  type: string
- description: Worker citizenship status
  name: Citizenship
  type: string
- description: ''
  name: Assignment
  type: object
- description: Record creation timestamp
  name: CreationDate
  type: string
- description: Last modification timestamp
  name: LastUpdateDate
  type: string
provider_name: Oracle Fusion Cloud Applications
provider_slug: oracle-fusion
schema_file: json-schema/oracle-fusion-worker-schema.json
slug: oracle-fusion-worker
source_filename: oracle-fusion-worker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/oracle-fusion/worker.json\",\n  \"title\": \"Oracle Fusion Cloud Worker\",\n  \"description\": \"A worker record in Oracle Fusion Cloud HCM representing an employee or contingent worker, including person details, employment information, and work assignments.\",\n  \"type\": \"object\",\n  \"required\": [\"FirstName\", \"LastName\"],\n  \"properties\": {\n    \"PersonId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique system-generated person identifier\"\n    },\n    \"PersonNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique person number assigned to the worker\"\n    },\n    \"FirstName\": {\n      \"type\": \"string\",\n      \"description\": \"Worker first name\",\n      \"minLength\": 1,\n      \"maxLength\": 150\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"description\": \"Worker last name\",\n\
  \      \"minLength\": 1,\n      \"maxLength\": 150\n    },\n    \"MiddleName\": {\n      \"type\": \"string\",\n      \"description\": \"Worker middle name\",\n      \"maxLength\": 60\n    },\n    \"DisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"Full formatted display name\"\n    },\n    \"DateOfBirth\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Worker date of birth\"\n    },\n    \"WorkEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary work email address\"\n    },\n    \"WorkPhoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Primary work phone number\"\n    },\n    \"HireDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Original hire date\"\n    },\n    \"EffectiveStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Effective start date of the current record\"\
  \n    },\n    \"WorkerType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Employee\", \"Contingent Worker\"],\n      \"description\": \"Classification of the worker relationship\"\n    },\n    \"PersonType\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed person type classification\"\n    },\n    \"Citizenship\": {\n      \"type\": \"string\",\n      \"description\": \"Worker citizenship status\"\n    },\n    \"Assignment\": {\n      \"$ref\": \"#/$defs/Assignment\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"LastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  },\n  \"$defs\": {\n    \"Assignment\": {\n      \"type\": \"object\",\n      \"description\": \"Work assignment details for the worker\",\n      \"properties\": {\n        \"AssignmentId\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Assignment identifier\"\n        },\n        \"AssignmentNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Assignment number\"\n        },\n        \"BusinessUnitName\": {\n          \"type\": \"string\",\n          \"description\": \"Business unit name\"\n        },\n        \"DepartmentName\": {\n          \"type\": \"string\",\n          \"description\": \"Department name\"\n        },\n        \"JobName\": {\n          \"type\": \"string\",\n          \"description\": \"Job title\"\n        },\n        \"PositionName\": {\n          \"type\": \"string\",\n          \"description\": \"Position name\"\n        },\n        \"GradeName\": {\n          \"type\": \"string\",\n          \"description\": \"Grade name\"\n        },\n        \"LocationName\": {\n          \"type\": \"string\",\n          \"description\": \"Work location\"\n        },\n        \"ManagerDisplayName\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Direct manager display name\"\n        },\n        \"AssignmentStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"Active\", \"Suspended\", \"Inactive\"],\n          \"description\": \"Current status of the assignment\"\n        },\n        \"EffectiveStartDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Assignment effective start date\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/json-schema/oracle-fusion-worker-schema.json
tags:
- Cloud
- CX
- Enterprise
- EPM
- ERP
- HCM
- Project Management
- REST API
- SaaS
- SCM
title: Oracle Fusion Cloud Worker
---
