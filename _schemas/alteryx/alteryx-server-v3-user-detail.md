---
description: Detailed representation of a user account
layout: schema
name: UserDetail
properties_list:
- description: Unique user identifier
  name: id
  type: string
- description: User's first name
  name: firstName
  type: string
- description: User's last name
  name: lastName
  type: string
- description: User's email address
  name: email
  type: string
- description: User role
  name: role
  type: string
- description: Date the user was created
  name: dateCreated
  type: string
- description: Default worker tag
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
- description: ''
  name: isAccountLocked
  type: boolean
- description: ''
  name: isActive
  type: boolean
- description: ''
  name: isValidated
  type: boolean
- description: ''
  name: timeZone
  type: string
- description: ''
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
schema_file: json-schema/alteryx-server-v3-user-detail-schema.json
slug: alteryx-server-v3-user-detail
source_filename: alteryx-server-v3-user-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserDetail\",\n  \"type\": \"object\",\n  \"description\": \"Detailed representation of a user account\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user identifier\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"User's first name\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"User's last name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"User's email address\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"User role\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"description\": \"Date the user was created\"\n    },\n    \"defaultWorkerTag\": {\n      \"type\": \"string\",\n      \"description\": \"Default worker tag\"\n    },\n    \"canScheduleJobs\": {\n      \"type\"\
  : \"boolean\"\n    },\n    \"canPrioritizeJobs\": {\n      \"type\": \"boolean\"\n    },\n    \"canAssignJobs\": {\n      \"type\": \"boolean\"\n    },\n    \"canCreateCollections\": {\n      \"type\": \"boolean\"\n    },\n    \"isApiEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"defaultCredentialId\": {\n      \"type\": \"string\"\n    },\n    \"isAccountLocked\": {\n      \"type\": \"boolean\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    },\n    \"isValidated\": {\n      \"type\": \"boolean\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\"\n    },\n    \"language\": {\n      \"type\": \"string\"\n    },\n    \"canCreateAndUpdateDcm\": {\n      \"type\": \"boolean\"\n    },\n    \"canShareForExecutionDcm\": {\n      \"type\": \"boolean\"\n    },\n    \"canShareForCollaborationDcm\": {\n      \"type\": \"boolean\"\n    },\n    \"canManageGenericVaultsDcm\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-user-detail-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: UserDetail
---
