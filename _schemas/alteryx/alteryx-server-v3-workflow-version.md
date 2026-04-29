---
description: A specific version of a workflow
layout: schema
name: WorkflowVersion
properties_list:
- description: Unique version identifier
  name: versionId
  type: string
- description: Sequential version number
  name: versionNumber
  type: integer
- description: Date the version was created
  name: dateCreated
  type: string
- description: Source from which the version was uploaded
  name: uploadSource
  type: string
- description: Date the version was uploaded
  name: uploadDate
  type: string
- description: Type of workflow in the package
  name: packageWorkflowType
  type: string
- description: Whether this version is the published version
  name: published
  type: boolean
- description: Comments about this version
  name: comments
  type: string
- description: Whether execution is disabled for this version
  name: runDisabled
  type: boolean
- description: ''
  name: executionMode
  type: string
- description: ''
  name: workflowCredentialType
  type: string
- description: Credential ID if workflowCredentialType is Specific
  name: credentialId
  type: string
- description: ''
  name: hasPrivateDataExemption
  type: boolean
- description: ''
  name: othersMayDownload
  type: boolean
- description: ''
  name: othersCanViewHistory
  type: boolean
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-workflow-version-schema.json
slug: alteryx-server-v3-workflow-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowVersion\",\n  \"type\": \"object\",\n  \"description\": \"A specific version of a workflow\",\n  \"properties\": {\n    \"versionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique version identifier\"\n    },\n    \"versionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Sequential version number\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"description\": \"Date the version was created\"\n    },\n    \"uploadSource\": {\n      \"type\": \"string\",\n      \"description\": \"Source from which the version was uploaded\"\n    },\n    \"uploadDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the version was uploaded\"\n    },\n    \"packageWorkflowType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of workflow in the package\"\n    },\n    \"published\": {\n      \"type\": \"boolean\",\n\
  \      \"description\": \"Whether this version is the published version\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Comments about this version\"\n    },\n    \"runDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether execution is disabled for this version\"\n    },\n    \"executionMode\": {\n      \"type\": \"string\"\n    },\n    \"workflowCredentialType\": {\n      \"type\": \"string\"\n    },\n    \"credentialId\": {\n      \"type\": \"string\",\n      \"description\": \"Credential ID if workflowCredentialType is Specific\"\n    },\n    \"hasPrivateDataExemption\": {\n      \"type\": \"boolean\"\n    },\n    \"othersMayDownload\": {\n      \"type\": \"boolean\"\n    },\n    \"othersCanViewHistory\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-workflow-version-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: WorkflowVersion
---
