---
description: Detailed representation of an Alteryx workflow including versions
layout: schema
name: WorkflowDetail
properties_list:
- description: Unique workflow identifier
  name: id
  type: string
- description: Source application identifier
  name: sourceAppId
  type: string
- description: Date the workflow was created
  name: dateCreated
  type: string
- description: Total number of times the workflow has been executed
  name: runCount
  type: integer
- description: List of workflow versions
  name: versions
  type: array
- description: Name of the workflow
  name: name
  type: string
- description: ID of the workflow owner
  name: ownerId
  type: string
- description: Worker tag for execution routing
  name: workerTag
  type: string
- description: District tags assigned to the workflow
  name: districtTags
  type: array
- description: Comments about the workflow
  name: comments
  type: string
- description: Whether the workflow is publicly accessible
  name: isPublic
  type: boolean
- description: Whether the workflow is ready for migration
  name: isReadyForMigration
  type: boolean
- description: ID of the currently published version
  name: publishedVersionId
  type: string
- description: Whether other users may download the workflow
  name: othersMayDownload
  type: boolean
- description: Whether other users can view execution history
  name: othersCanViewHistory
  type: boolean
- description: Whether other users can execute the workflow
  name: othersCanExecute
  type: boolean
- description: Whether the workflow has a private data exemption
  name: hasPrivateDataExemption
  type: boolean
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-workflow-detail-schema.json
slug: alteryx-server-v3-workflow-detail
source_filename: alteryx-server-v3-workflow-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowDetail\",\n  \"type\": \"object\",\n  \"description\": \"Detailed representation of an Alteryx workflow including versions\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique workflow identifier\"\n    },\n    \"sourceAppId\": {\n      \"type\": \"string\",\n      \"description\": \"Source application identifier\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"description\": \"Date the workflow was created\"\n    },\n    \"runCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of times the workflow has been executed\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"List of workflow versions\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"ID of the workflow owner\"\n    },\n    \"workerTag\": {\n      \"type\": \"string\",\n      \"description\": \"Worker tag for execution routing\"\n    },\n    \"districtTags\": {\n      \"type\": \"array\",\n      \"description\": \"District tags assigned to the workflow\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Comments about the workflow\"\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workflow is publicly accessible\"\n    },\n    \"isReadyForMigration\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workflow is ready for migration\"\n    },\n    \"publishedVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the currently published version\"\n    },\n    \"othersMayDownload\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether other users may download the workflow\"\n    },\n    \"othersCanViewHistory\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether other users can view execution history\"\n    },\n    \"othersCanExecute\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether other users can execute the workflow\"\n    },\n    \"hasPrivateDataExemption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workflow has a private data exemption\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-workflow-detail-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: WorkflowDetail
---
