---
description: Metadata details for a workflow version
layout: schema
name: WorkflowVersionDetails
properties_list:
- description: Whether the version uses AMP engine
  name: isAmp
  type: boolean
- description: Name of the workflow file
  name: fileName
  type: string
- description: Author of the workflow
  name: author
  type: string
- description: Copyright information
  name: copyright
  type: string
- description: Description of the workflow
  name: description
  type: string
- description: Display name of the workflow
  name: name
  type: string
- description: Message shown when no output files are generated
  name: noOutputFilesMessage
  type: string
- description: Message shown with output files
  name: outputMessage
  type: string
- description: Related URL
  name: url
  type: string
- description: Display text for the related URL
  name: urlText
  type: string
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-workflow-version-details-schema.json
slug: alteryx-server-v3-workflow-version-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowVersionDetails\",\n  \"type\": \"object\",\n  \"description\": \"Metadata details for a workflow version\",\n  \"properties\": {\n    \"isAmp\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the version uses AMP engine\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow file\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Author of the workflow\"\n    },\n    \"copyright\": {\n      \"type\": \"string\",\n      \"description\": \"Copyright information\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the workflow\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the workflow\"\n    },\n    \"noOutputFilesMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Message\
  \ shown when no output files are generated\"\n    },\n    \"outputMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Message shown with output files\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Related URL\"\n    },\n    \"urlText\": {\n      \"type\": \"string\",\n      \"description\": \"Display text for the related URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-workflow-version-details-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: WorkflowVersionDetails
---
