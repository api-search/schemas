---
description: Contract for updating an existing user
layout: schema
name: UpdateUserContract
properties_list:
- description: User ID (optional, for verification)
  name: id
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: role
  type: string
- description: ''
  name: defaultWorkerTag
  type: string
- description: ''
  name: canScheduleJobs
  type: boolean
- description: ''
  name: canPrioritizeJobs
  type: boolean
- description: ''
  name: canAssignJobs
  type: boolean
- description: ''
  name: canCreateCollections
  type: boolean
- description: ''
  name: isApiEnabled
  type: boolean
- description: ''
  name: defaultCredentialId
  type: string
- description: Whether the account is locked
  name: isAccountLocked
  type: boolean
- description: ''
  name: isActive
  type: boolean
- description: Whether the user's email has been validated
  name: isValidated
  type: boolean
- description: ''
  name: timeZone
  type: string
- description: User's preferred language
  name: language
  type: string
- description: ''
  name: canCreateAndUpdateDcm
  type: boolean
- description: ''
  name: canShareForExecutionDcm
  type: boolean
- description: ''
  name: canShareForCollaborationDcm
  type: boolean
- description: ''
  name: canManageGenericVaultsDcm
  type: boolean
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-update-user-contract-schema.json
slug: alteryx-server-v3-update-user-contract
source_filename: alteryx-server-v3-update-user-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateUserContract\",\n  \"type\": \"object\",\n  \"description\": \"Contract for updating an existing user\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User ID (optional, for verification)\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"role\": {\n      \"type\": \"string\"\n    },\n    \"defaultWorkerTag\": {\n      \"type\": \"string\"\n    },\n    \"canScheduleJobs\": {\n      \"type\": \"boolean\"\n    },\n    \"canPrioritizeJobs\": {\n      \"type\": \"boolean\"\n    },\n    \"canAssignJobs\": {\n      \"type\": \"boolean\"\n    },\n    \"canCreateCollections\": {\n      \"type\": \"boolean\"\n    },\n    \"isApiEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"defaultCredentialId\": {\n      \"\
  type\": \"string\"\n    },\n    \"isAccountLocked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account is locked\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    },\n    \"isValidated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user's email has been validated\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"User's preferred language\"\n    },\n    \"canCreateAndUpdateDcm\": {\n      \"type\": \"boolean\"\n    },\n    \"canShareForExecutionDcm\": {\n      \"type\": \"boolean\"\n    },\n    \"canShareForCollaborationDcm\": {\n      \"type\": \"boolean\"\n    },\n    \"canManageGenericVaultsDcm\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-update-user-contract-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: UpdateUserContract
---
