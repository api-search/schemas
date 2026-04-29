---
description: Contract for updating an existing workflow
layout: schema
name: UpdateWorkflowContract
properties_list:
- description: Updated workflow name
  name: name
  type: string
- description: Version ID to update
  name: versionId
  type: string
- description: Whether to make the specified version published
  name: makePublished
  type: boolean
- description: Updated owner ID
  name: ownerId
  type: string
- description: Updated worker tag
  name: workerTag
  type: string
- description: Updated district tags
  name: districtTags
  type: array
- description: Updated comments
  name: comments
  type: string
- description: ''
  name: isPublic
  type: boolean
- description: ''
  name: isReadyForMigration
  type: boolean
- description: ''
  name: othersMayDownload
  type: boolean
- description: ''
  name: othersCanExecute
  type: boolean
- description: ''
  name: executionMode
  type: string
- description: ''
  name: hasPrivateDataExemption
  type: boolean
- description: ''
  name: workflowCredentialType
  type: string
- description: ''
  name: credentialId
  type: string
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-update-workflow-contract-schema.json
slug: alteryx-server-v3-update-workflow-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateWorkflowContract\",\n  \"type\": \"object\",\n  \"description\": \"Contract for updating an existing workflow\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Updated workflow name\"\n    },\n    \"versionId\": {\n      \"type\": \"string\",\n      \"description\": \"Version ID to update\"\n    },\n    \"makePublished\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to make the specified version published\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"Updated owner ID\"\n    },\n    \"workerTag\": {\n      \"type\": \"string\",\n      \"description\": \"Updated worker tag\"\n    },\n    \"districtTags\": {\n      \"type\": \"array\",\n      \"description\": \"Updated district tags\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Updated comments\"\
  \n    },\n    \"isPublic\": {\n      \"type\": \"boolean\"\n    },\n    \"isReadyForMigration\": {\n      \"type\": \"boolean\"\n    },\n    \"othersMayDownload\": {\n      \"type\": \"boolean\"\n    },\n    \"othersCanExecute\": {\n      \"type\": \"boolean\"\n    },\n    \"executionMode\": {\n      \"type\": \"string\"\n    },\n    \"hasPrivateDataExemption\": {\n      \"type\": \"boolean\"\n    },\n    \"workflowCredentialType\": {\n      \"type\": \"string\"\n    },\n    \"credentialId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-update-workflow-contract-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: UpdateWorkflowContract
---
