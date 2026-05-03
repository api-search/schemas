---
description: Schema for submitting, approving, or rejecting Salesforce approval process requests.
layout: schema
name: Salesforce Approval Request
properties_list:
- description: Array of approval actions to perform.
  name: requests
  type: array
provider_name: Salesforce Automation System
provider_slug: salesforce-automation-system
schema_file: json-schema/salesforce-approval-request-schema.json
slug: salesforce-approval-request
source_filename: salesforce-approval-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salesforce-automation-system/json-schema/salesforce-approval-request-schema.json\",\n  \"title\": \"Salesforce Approval Request\",\n  \"description\": \"Schema for submitting, approving, or rejecting Salesforce approval process requests.\",\n  \"type\": \"object\",\n  \"required\": [\"requests\"],\n  \"properties\": {\n    \"requests\": {\n      \"type\": \"array\",\n      \"description\": \"Array of approval actions to perform.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"actionType\", \"contextActorId\", \"contextId\"],\n        \"properties\": {\n          \"actionType\": {\n            \"type\": \"string\",\n            \"enum\": [\"Submit\", \"Approve\", \"Reject\", \"Recall\", \"Reassign\"],\n            \"description\": \"The type of approval action to perform.\"\n          },\n          \"contextActorId\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"ID of the Salesforce user performing the action.\"\n          },\n          \"contextId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the record being submitted for approval or acted upon.\"\n          },\n          \"comments\": {\n            \"type\": \"string\",\n            \"description\": \"Optional comments explaining the approval decision.\"\n          },\n          \"nextApproverIds\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" },\n            \"description\": \"IDs of users to assign as next approvers (for manual approver routing).\"\n          },\n          \"processDefinitionNameOrId\": {\n            \"type\": \"string\",\n            \"description\": \"Name or ID of the approval process to use when submitting (for Submit actions).\"\n          },\n          \"skipEntryCriteria\": {\n            \"type\": \"boolean\",\n           \
  \ \"description\": \"Whether to skip approval process entry criteria evaluation.\",\n            \"default\": false\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-automation-system/refs/heads/main/json-schema/salesforce-approval-request-schema.json
tags:
- Approval Process
- Automation
- CRM
- Flow
- Process Builder
- Salesforce
- Workflow
title: Salesforce Approval Request
---
