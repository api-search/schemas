---
description: ''
layout: schema
name: ProcessApprovalsSubmitRequest
properties_list:
- description: ''
  name: actionType
  type: string
- description: ''
  name: contextActorId
  type: string
- description: ''
  name: contextId
  type: string
- description: ''
  name: comments
  type: string
- description: ''
  name: nextApproverIds
  type: string
- description: ''
  name: processDefinitionNameOrId
  type: string
- description: ''
  name: skipEntryCriteria
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-process-approvals-submit-request-schema.json
slug: salesforce-process-approvals-submit-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contextActorId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"contextId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"nextApproverIds\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"processDefinitionNameOrId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"skipEntryCriteria\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"actionType\",\n    \"contextActorId\",\n    \"contextId\",\n    \"comments\",\n    \"nextApproverIds\",\n    \"processDefinitionNameOrId\",\n    \"skipEntryCriteria\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ProcessApprovalsSubmitRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-process-approvals-submit-request-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: ProcessApprovalsSubmitRequest
---
