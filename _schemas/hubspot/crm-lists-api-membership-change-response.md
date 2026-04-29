---
description: Response from a list membership change operation.
layout: schema
name: MembershipChangeResponse
properties_list:
- description: ''
  name: recordIdsAdded
  type: array
- description: ''
  name: recordIdsAlreadyMember
  type: array
- description: ''
  name: recordIdsRemoved
  type: array
- description: ''
  name: recordIdsMissing
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-lists-api-membership-change-response-schema.json
slug: crm-lists-api-membership-change-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-lists-api-membership-change-response-schema.json\",\n  \"title\": \"MembershipChangeResponse\",\n  \"description\": \"Response from a list membership change operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recordIdsAdded\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"500123\"\n      ]\n    },\n    \"recordIdsAlreadyMember\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"500123\"\n      ]\n    },\n    \"recordIdsRemoved\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"500123\"\n      ]\n    },\n    \"recordIdsMissing\": {\n      \"type\": \"array\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"500123\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-lists-api-membership-change-response-schema.json
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
title: MembershipChangeResponse
---
