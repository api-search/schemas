---
description: Contract for creating a new user
layout: schema
name: CreateUserContract
properties_list:
- description: User's first name
  name: firstName
  type: string
- description: User's last name
  name: lastName
  type: string
- description: User's email address
  name: email
  type: string
- description: User role determining access level
  name: role
  type: string
- description: Default worker tag for the user
  name: defaultWorkerTag
  type: string
- description: Whether the user can create schedules
  name: canScheduleJobs
  type: boolean
- description: Whether the user can set job priority
  name: canPrioritizeJobs
  type: boolean
- description: Whether the user can assign jobs to workers
  name: canAssignJobs
  type: boolean
- description: Whether the user can create collections
  name: canCreateCollections
  type: boolean
- description: Whether API access is enabled for the user
  name: isApiEnabled
  type: boolean
- description: Default credential ID for the user
  name: defaultCredentialId
  type: string
- description: Whether the user account is active
  name: isActive
  type: boolean
- description: User's preferred time zone
  name: timeZone
  type: string
- description: Whether the user can create and update DCM connections
  name: canCreateAndUpdateDcm
  type: boolean
- description: Whether the user can share DCM connections for execution
  name: canShareForExecutionDcm
  type: boolean
- description: Whether the user can share DCM connections for collaboration
  name: canShareForCollaborationDcm
  type: boolean
- description: Whether the user can manage generic DCM vaults
  name: canManageGenericVaultsDcm
  type: boolean
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-create-user-contract-schema.json
slug: alteryx-server-v3-create-user-contract
source_filename: alteryx-server-v3-create-user-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateUserContract\",\n  \"type\": \"object\",\n  \"description\": \"Contract for creating a new user\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"User's first name\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"User's last name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"User's email address\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"User role determining access level\"\n    },\n    \"defaultWorkerTag\": {\n      \"type\": \"string\",\n      \"description\": \"Default worker tag for the user\"\n    },\n    \"canScheduleJobs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can create schedules\"\n    },\n    \"canPrioritizeJobs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the user can set job priority\"\n    },\n    \"canAssignJobs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can assign jobs to workers\"\n    },\n    \"canCreateCollections\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can create collections\"\n    },\n    \"isApiEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether API access is enabled for the user\"\n    },\n    \"defaultCredentialId\": {\n      \"type\": \"string\",\n      \"description\": \"Default credential ID for the user\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"User's preferred time zone\"\n    },\n    \"canCreateAndUpdateDcm\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can create and update DCM connections\"\n    },\n    \"canShareForExecutionDcm\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can share DCM connections for execution\"\n    },\n    \"canShareForCollaborationDcm\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can share DCM connections for collaboration\"\n    },\n    \"canManageGenericVaultsDcm\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can manage generic DCM vaults\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-create-user-contract-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: CreateUserContract
---
