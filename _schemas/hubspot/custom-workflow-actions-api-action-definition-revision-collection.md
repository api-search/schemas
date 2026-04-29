---
description: A paginated collection of action definition revisions
layout: schema
name: ActionDefinitionRevisionCollection
properties_list:
- description: List of revisions
  name: results
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/custom-workflow-actions-api-action-definition-revision-collection-schema.json
slug: custom-workflow-actions-api-action-definition-revision-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-definition-revision-collection-schema.json\",\n  \"title\": \"ActionDefinitionRevisionCollection\",\n  \"description\": \"A paginated collection of action definition revisions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of revisions\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A revision of an action definition\",\n        \"required\": [\n          \"revisionId\",\n          \"definition\",\n          \"createdAt\"\n        ],\n        \"properties\": {\n          \"revisionId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the revision\",\n            \"example\": \"500123\"\n          },\n          \"definition\"\
  : {\n            \"$ref\": \"#/components/schemas/ActionDefinition\"\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"When the revision was created\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"revisionId\": \"500123\",\n          \"definition\": {},\n          \"createdAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the next page\"\n            }\n          },\n          \"example\": {\n            \"after\": \"example-value\"\n          }\n        }\n      }\n    }\n  },\n  \"required\"\
  : [\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/custom-workflow-actions-api-action-definition-revision-collection-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: ActionDefinitionRevisionCollection
---
