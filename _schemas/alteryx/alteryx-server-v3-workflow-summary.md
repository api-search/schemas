---
description: Summary representation of an Alteryx workflow
layout: schema
name: WorkflowSummary
properties_list:
- description: Unique workflow identifier
  name: id
  type: string
- description: Source application identifier for migration tracking
  name: sourceAppId
  type: string
- description: Name of the workflow
  name: name
  type: string
- description: ID of the workflow owner
  name: ownerId
  type: string
- description: Date the workflow was created (ISO 8601)
  name: dateCreated
  type: string
- description: Version number of the published version
  name: publishedVersionNumber
  type: integer
- description: Whether the workflow uses AMP engine
  name: isAmp
  type: boolean
- description: Execution mode for the workflow
  name: executionMode
  type: string
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-workflow-summary-schema.json
slug: alteryx-server-v3-workflow-summary
source_filename: alteryx-server-v3-workflow-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary representation of an Alteryx workflow\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique workflow identifier\"\n    },\n    \"sourceAppId\": {\n      \"type\": \"string\",\n      \"description\": \"Source application identifier for migration tracking\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the workflow owner\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"description\": \"Date the workflow was created (ISO 8601)\"\n    },\n    \"publishedVersionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the published version\"\n    },\n    \"isAmp\": {\n      \"type\":\
  \ \"boolean\",\n      \"description\": \"Whether the workflow uses AMP engine\"\n    },\n    \"executionMode\": {\n      \"type\": \"string\",\n      \"description\": \"Execution mode for the workflow\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-workflow-summary-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: WorkflowSummary
---
